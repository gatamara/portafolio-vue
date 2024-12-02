<template>
  <div id="contacto"
    class="w-full p-32 text-center  border border-purple-200 shadow  dark:bg-slate-900 dark:border-purple-700">
    <h5 class="mb-2 text-4xl font-semibold text-purple-900 dark:text-white">Contactame</h5>
    <p class="mb-5 text-base text-purple-500 sm:text-lg dark:text-purple-400">Me puedes encontrar en redes como
      Linkedin,
      correo electronico y ver mis respositorios en Github.</p>
    <div class="items-center justify-center space-y-4 sm:flex sm:space-y-0 sm:space-x-4 rtl:space-x-reverse">

      <a href="https://www.linkedin.com/in/gatamara/"
        class="w-full sm:w-auto bg-purple-800 hover:bg-purple-700 focus:ring-4 focus:outline-none focus:ring-purple-300 text-white rounded-lg inline-flex items-center justify-center px-4 py-2.5 dark:bg-purple-700 dark:hover:bg-purple-600 dark:focus:ring-purple-700">

        <FontAwesomeIcon :icon="faLinkedin" />
        <div class="text-left rtl:text-right">
          <div class="p-4 font-sans text-sm font-semibold">Likedin </div>
        </div>
      </a>
      <a href="#"
        class="w-full sm:w-auto bg-purple-800 hover:bg-purple-700 focus:ring-4 focus:outline-none focus:ring-purple-300 text-white rounded-lg inline-flex items-center justify-center px-4 py-2.5 dark:bg-purple-700 dark:hover:bg-purple-600 dark:focus:ring-purple-700">
        <FontAwesomeIcon :icon="faEnvelope" />
        <div class="text-left rtl:text-right">
          <div class="p-4 font-sans text-sm font-semibold">Email </div>
        </div>
      </a>
    </div>
  </div>
</template>

<script setup>
import { faLinkedin } from '@fortawesome/free-brands-svg-icons';
import { faEnvelope } from '@fortawesome/free-solid-svg-icons';
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';

</script>
