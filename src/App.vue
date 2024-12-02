<script setup>
import ContactMe from './components/ContactMe.vue';
import MyBanner from './components/MyBanner.vue';
import MySkills from './components/MySkills.vue';
import MyWorks from './components/MyWorks.vue';
import NavBar from './components/NavBar.vue';


</script>

<template>
  <header>
    <NavBar />
  </header>
  <main class="bg-slate-900 ">
    <MyBanner />
    <MySkills />
    <MyWorks />

  </main>
  <ContactMe />


</template>

<style scoped></style>
