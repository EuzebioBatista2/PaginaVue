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
    flex-wrap: wrap;
    padding: 0px 80px;
  }

</style>