<template>
  <div class="vuokemon-container">
    <img class="fade-in hidden-vuokemon" :src="srcImg" />
    <img class="fade-in" :src="srcImg" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      vuemonId: 5,
      srcImg: "",
    };
  },
  methods: {
    obtenerImagen() {
      this.srcImg = `https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/other/dream-world/${this.vuemonId}.svg`;
    },
  },
  mounted() {
    this.obtenerImagen();
  },
};
</script>

<style scoped>
.vuokemon-container {
  height: 200px;
}

img {
  height: 200px;
  user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  -webkit-user-drag: none;
  -webkit-user-select: none;
}

.hidden-vuokemon {
  filter: brightness(0);
}
</style>