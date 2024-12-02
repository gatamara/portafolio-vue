<template>
  <div id="skills" class="max-w-6xl mx-auto p-10">
    <h1 class="text-center text-white text-4xl font-semibold pb-14">Skills</h1>
    <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 gap-8 my-8">
      <div class="flex flex-col justify-center items-center gap-2">
        <FontAwesomeIcon :icon="faCss3Alt" class="custom-size" />
        <h4 class="text-white text-2xl">CSS</h4>
      </div>
      <div class="flex flex-col justify-center items-center gap-2">
        <FontAwesomeIcon :icon="faHtml5" class="custom-size" />
        <h4 class="text-white text-2xl">HTML</h4>
      </div>
      <div class="flex flex-col justify-center items-center gap-2">
        <FontAwesomeIcon :icon="faJs" class="custom-size" />
        <h4 class="text-white text-2xl">JavaScript</h4>
      </div>
      <div class="flex flex-col justify-center items-center gap-2">
        <FontAwesomeIcon :icon="faVuejs" class="custom-size" />
        <h4 class="text-white text-2xl">VueJs</h4>
      </div>
      <div class="flex flex-col justify-center items-center gap-2">
        <FontAwesomeIcon :icon="faReact" class="custom-size" />
        <h4 class="text-white text-2xl">ReactJs</h4>
      </div>
      <div class="flex flex-col justify-center items-center gap-2">
        <FontAwesomeIcon :icon="faGithub" class="custom-size" />
        <h4 class="text-white text-2xl">Github</h4>
      </div>
      <div class="flex flex-col justify-center items-center gap-2">
        <FontAwesomeIcon :icon="faGitAlt" class="custom-size" />
        <h4 class="text-white text-2xl">Git</h4>
      </div>
      <div class="flex flex-col justify-center items-center gap-2">
        <FontAwesomeIcon :icon="faT" class="custom-size" />
        <h4 class="text-white text-2xl">TypeScript</h4>
      </div>
      <div class="flex flex-col justify-center items-center gap-2">
        <FontAwesomeIcon :icon="faBootstrap" class="custom-size" />
        <h4 class="text-white text-2xl">Bootstrap</h4>
      </div>
      <div class="flex flex-col justify-center items-center gap-2 ">
        <TailwindLogo />
        <h4 class="text-white text-2xl">Tailwind</h4>
      </div>
    </div>
  </div>
</template>

<script setup>
import { faBootstrap, faCss3Alt, faGitAlt, faGithub, faHtml5, faJs, faReact, faVuejs } from '@fortawesome/free-brands-svg-icons';
import { faT } from '@fortawesome/free-solid-svg-icons';
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
import TailwindLogo from './icons/TailwindLogo.vue';
</script>

<style scoped>
.custom-size {
  font-size: 70px;
  color: rgb(169, 151, 226);
}
</style>
