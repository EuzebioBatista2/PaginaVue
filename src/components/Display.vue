<template>
  <div class="display">
      <Header />
  </div>
</template>

<script>
import Header from './Header.vue';
export default {
    components: { Header }

}
</script>

<style>
    .display {
        display: flex;
        margin: 40px;
    }
    

</style>