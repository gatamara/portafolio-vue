<template>
  <div class="card">
    <div class="poster">
      <img :src="image" alt="Project Image" class="card-img" />
    </div>
    <div class="details">
      <h2 class="text-lg font-medium">{{ title }}</h2>
      <p>{{ description }}</p>
      <div class="logos-project">
        <slot name="logos"></slot>
      </div>
      <div class="buttons-view">
        <button v-for="(button, index) in buttons" :key="index" class="button" :style="{
          backgroundColor: button.backgroundColor,
          color: button.color,
          borderColor: button.borderColor,
        }" @click="goTo(button.href)">
          <slot :name="`icon-${index}`">{{ button.icon }}</slot>
          {{ button.text }}
        </button>
      </div>
    </div>
  </div>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "CardWork",
  props: {
    image: {
      type: String,
      required: true,
    },
    title: {
      type: String,
      required: true,
    },
    description: {
      type: String,
      required: true,
    },
    buttons: {
      type: Array,
      required: true,
    },
  },
  setup() {
    const goTo = (href) => {
      window.open(href, "_blank");
    };
    return { goTo };
  },
});
</script>

<style scoped>
.card {
  position: relative;
  width: 350px;
  height: 350px;
  border-radius: 8px;
  box-shadow: 0 15px 35px rgba(255, 255, 255, 0.2);
  cursor: pointer;
  overflow: hidden;
}


.card .poster::before {
  content: '';
  position: absolute;
  bottom: -100px;
  width: 100%;
  height: 100%;
  background: linear-gradient(0deg, #532663 70%, transparent);
  transition: 0.5s;
  z-index: 1;
}

.card:hover .poster::before {
  bottom: -10px;
}

.card-img {
  width: 100%;
  transition: 0.5s;
}

.card:hover .card-img {
  transform: translateY(-50px);
  filter: blur(5px);
}

.card .details {
  position: absolute;
  bottom: 10px;
  left: 0;
  padding: 16px;
  z-index: 2;
  transition: 0.5s;
  color: #fff;
}

.card:hover .details {
  bottom: 0px;
}

.card .details h2 {
  color: #fff;
  display: flex;
  justify-content: space-around;
}

.card .details p {
  max-width: 300px;
  text-align: center;
  opacity: 0.8;
}


.card .details .buttons-view {
  position: relative;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  gap: 24px;
  padding-top: 8px;
}

.button {
  cursor: pointer;
  padding: 8px 16px;
  border: 1px solid;
  border-radius: 4px;
  text-align: center;
  transition: all 0.3s ease;
}

.button:hover {
  opacity: 0.5;
}
</style>
