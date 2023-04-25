<template>
  <section class="container-section">
    <Card layout="facebook" />
    <Card layout="instagram" />
    <Card layout="linkedin" />
    <Card layout="discord" />
    <Card layout="github" />
    <Card layout="telegram" />
  </section>
</template>

<script>
import Card from './Card.vue';
export default {
  name: "Section",
  components: { Card }

}
</script>

<style>
  .container-section {
    display: flex;
    box-sizing: border-box;
    flex-wrap: wrap;
    width: 100%;
    padding: 2.0rem 0;
  }

</style>