<template>
  <h2>Coche - Composition Api</h2>
  <p>Marca: {{ brand }}</p>
  <p>Modelo: {{ model }}</p>
</template>

<script>

export default {
  props:{
    power: {
      type: Number,
      default: 60,
    },

  },
  setup() {
    const brand = "Audi";
    const model = "A4";

    return {
      brand,
      model,
    };
  },
};
</script>

<style></style>
