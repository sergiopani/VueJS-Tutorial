<template>
  <h1>Vue JS</h1>
  <Car :power="power"/>
</template>

<script>
import Car from "./components/Car";
export default {
  components: {
    Car,
  },
  setup() {
    let power = 30;
    return {
      power,
    };
  },
};
</script>

<style></style>
