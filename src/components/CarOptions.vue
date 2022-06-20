<template>
  <h2>Coche - Options API</h2>
  <p>Marca: {{ brand }}</p>
  <p>Modelo: {{ model }}</p>
  <p>Potencia: {{ power }}</p>

  <button @click="upPower(1000)">Aumentar</button>
  <button @click="downPower">Disminuir</button>
</template>

<script>
export default {
  data() {
    return {
      brand: "Seat",
      model: "Leon",
      power: 50,
    };
  },
  methods: {
    upPower(newPower) {
      console.log("Aumentando potencia! -> " + newPower);
    },
    downPower() {
      console.log("Disminuyendo potencia!");
    },
  },
};
</script>

<style></style>
