<template>
  <div class="display">
      <Header />
      <Nav />
      <Section />
  </div>
</template>

<script>
import Header from './Header.vue';
import Nav from './Nav.vue'
import Section from './Section.vue';
export default {
    components: { Header, Nav, Section }

}
</script>

<style>
    .display {
        display: flex;
        flex-direction: column;
        margin: 0 50px;
    }
    

</style>