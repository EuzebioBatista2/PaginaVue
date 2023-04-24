<template>
  <div class="display">
      <Header />
      <Nav />
      <Section />
      <Footer />
  </div>
</template>

<script>
import Header from './Header.vue';
import Nav from './Nav.vue'
import Section from './Section.vue';
import Footer from './Footer.vue';
export default {
    components: { Header, Nav, Section, Footer }

}
</script>

<style>
    .display {
        max-width: 1200px;
    }
    

</style>