<template>
  <h2>Coche - Composition Api</h2>
  <p>Marca: {{ brand }}</p>
  <p>Modelo: {{ model }}</p>
  <p>Potencias urbanas menor de 300cv</p>
  <ul>
    <!--<li v-for="(power, index) in powers" :key="index">
      <template v-if="power < 300">{{ power }}</template>
    </li>-->
    <template v-for="(power, index) in powers" :key="index">
      <li v-if="power < 300">{{ power }}</li>
    </template>
  </ul>
  <p>Potencias urbanas mayores de 300cv</p>
  <ul>
    <template v-for="(power, index) in powers" :key="index">
      <li v-if="power >= 300">{{ power }}</li>
    </template>
  </ul>
</template>

<script>
export default {
  setup() {
    const brand = "Audi";
    const model = "A4";
    const powers = [60, 80, 120, 160, 200, 280, 300, 390, 540, 500];

    return {
      brand,
      model,
      powers,
    };
  },
};
</script>

<style></style>
