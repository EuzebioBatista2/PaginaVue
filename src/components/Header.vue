<template>
  <header class="header">
    <Icone />
    <h2>&nbsp;| Help center</h2>
  </header>
</template>

<script>
import Icone from "./Icone.vue"
export default {
  components: { Icone }
}
</script>

<style>
  .header {
    width: 100%;
    display: flex;
    border-top-right-radius: 10px;
    border-top-left-radius: 10px;
    align-items: center;
    background-color: #000 ;
    padding: 10px;
  }
  .header h2 {
    color: #fff;
    margin: 0;
    font-size: 1.5em;
    font-weight: 100;
  }

</style>