<template>
  <div class="relative h-[600px] w-full">
    <div class="absolute inset-0 bg-overlay"></div>
    <div class="relative z-10 flex items-center justify-center h-full ">
      <div class="w-4/5">
        <h3 class="text-white text-2xl pb-5 italic"> Hola! mi nombre es </h3>
        <h1
          class="text-5xl font-bold pb-10 bg-gradient-to-r from-fuchsia-200 to-rose-500 bg-clip-text text-transparent">
          Tamara
          Salinas
        </h1>
        <h1
          class="text-5xl font-bold pb-10 bg-gradient-to-r from-indigo-300 to-fuchsia-700 bg-clip-text text-transparent">
          Desarrolladora Front-end</h1>

        <p class="text-white font-medium line-clamp-3 leading-relaxed text-justify w-3/6"> Desarrolladora frontend con
          experiencia en la creación de
          interfaces de usuario atractivas y funcionales.
          Poseo habilidades sólidas en <strong class="underline decoration-sky-500">HTML</strong> , CSS, JavaScript,
          TypeScript, VueJs, ReactJs y Next.js, me gusta utilizar mi
          conocimiento para construir experiencias web de alta calidad.
        </p>

      </div>

    </div>
  </div>
</template>

<script setup>

</script>

<style scoped>
.bg-overlay {
  background-image: url('./fondo.jpg');
  background-size: cover;
  background-position: center;
  opacity: 0.3;
  z-index: 0;
}
</style>
