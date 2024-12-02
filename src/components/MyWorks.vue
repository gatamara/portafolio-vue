<template>
  <div id="trabajos" class=" p-20 bg-slate-800">
    <h1 class="text-center text-purple-400 text-4xl font-semibold pb-20">Proyectos VueJs</h1>
    <div class="container-card">
      <CardWork image="/modulo7.png" title="< Contador >" description="Creacion de contador con Vuex y test unitarios"
        :buttons="[
          { text: 'Ver', href: 'https://prueba-modulo7-tamara.web.app/', color: '#c084fc', backgroundColor: 'transparent', borderColor: '#c084fc' },
          { text: 'Repo GitHub', href: 'https://github.com/gatamara/prueba-modulo7', color: '#c084fc', backgroundColor: 'transparent', borderColor: '#c084fc' }
        ]">
        <template #logos>
          <div id="logos">
            <FontAwesomeIcon :icon="faJs" />
            <FontAwesomeIcon :icon="faHtml5" />
            <FontAwesomeIcon :icon="faCss3Alt" />
            <FontAwesomeIcon :icon="faVuejs" />
          </div>

        </template>
      </CardWork>
      <!-- card -->
      <CardWork image="/inde.png" title="< Indecision App >"
        description="Chat con respuesta automatica, utilizacion de peticion a Api" :buttons="[
          { text: 'Ver', href: 'https://github.com/gatamara/indecisionApp', color: '#c084fc', backgroundColor: 'transparent', borderColor: '#c084fc' },
          { text: 'Repo GitHub', href: 'https://github.com/gatamara/indecisionApp', color: '#c084fc', backgroundColor: 'transparent', borderColor: '#c084fc' }
        ]">
        <template #logos>
          <div id="logos">
            <FontAwesomeIcon :icon="faJs" />
            <FontAwesomeIcon :icon="faHtml5" />
            <FontAwesomeIcon :icon="faCss3Alt" />
            <FontAwesomeIcon :icon="faVuejs" />
          </div>
        </template>
      </CardWork>
      <CardWork image="/login.png" title="< Login >"
        description="Login y register, rutas protegidas con Vuex y VueRouter" :buttons="[
          { text: 'Ver', href: 'https://prueba-modulo7-tamara.web.app/', color: '#c084fc', backgroundColor: 'transparent', borderColor: '#c084fc' },
          { text: 'Repo GitHub', href: 'https://github.com/gatamara/prueba-modulo7', color: '#c084fc', backgroundColor: 'transparent', borderColor: '#c084fc' }
        ]">
        <template #logos>
          <div id="logos">
            <FontAwesomeIcon :icon="faJs" />
            <FontAwesomeIcon :icon="faHtml5" />
            <FontAwesomeIcon :icon="faCss3Alt" />
            <FontAwesomeIcon :icon="faVuejs" />
          </div>

        </template>
      </CardWork>
      <!-- card -->
      <CardWork image="/router.png" title="< VueRouter >"
        description="Integracion de  VueRouter a proyecto con Bootstrap" :buttons="[
          { text: 'Ver', href: 'https://prueba-modulo7-tamara.web.app/', color: '#c084fc', backgroundColor: 'transparent', borderColor: '#c084fc' },
          { text: 'Repo GitHub', href: 'https://github.com/gatamara/prueba-modulo7', color: '#c084fc', backgroundColor: 'transparent', borderColor: '#c084fc' }
        ]">
        <template #logos>
          <div id="logos">
            <FontAwesomeIcon :icon="faJs" />
            <FontAwesomeIcon :icon="faHtml5" />
            <FontAwesomeIcon :icon="faCss3Alt" />
            <FontAwesomeIcon :icon="faVuejs" />
          </div>

        </template>
      </CardWork>

    </div>
  </div>

</template>
<script setup>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
import CardWork from './CardWork.vue';
import { faCss3Alt, faHtml5, faJs, faVuejs } from '@fortawesome/free-brands-svg-icons';

</script>
<style scoped>
.container-card {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 40px;
}

#logos {
  width: 100%;
  display: flex;
  justify-content: center;
  gap: 16px;
  font-size: 24px;
  padding: 4px;
}
</style>
