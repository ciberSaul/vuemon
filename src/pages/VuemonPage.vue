<template>
  <h1>¿Qué Vuemon es?</h1>
  <VuemonImg />
  <VuemonOpciones />
</template>

<script>
import VuemonOpciones from "@/components/VuemonOpciones.vue";
import VuemonImg from "@/components/VuemonImg.vue";
export default {
  components: {
    VuemonOpciones,
    VuemonImg,
  },
};
</script>

<style>
</style>