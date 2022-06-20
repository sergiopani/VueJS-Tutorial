<template>
  <h1>Vue JS</h1>
  <CarComposition />
  <hr/>
  <CarOptions />
</template>

<script>
import CarComposition from "./components/CarComposition";
import CarOptions from "./components/CarOptions";
export default {
  components: {
    CarComposition,
    CarOptions,
  },
};
</script>

<style></style>
