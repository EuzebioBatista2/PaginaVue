<template>
  <header class="header">
    <div class="container">
      <Icone />
      <h2>&nbsp;| Help center</h2>
    </div>
    <div class="container">
      <Button class="black" label="Submit a request" />
      <Button class="white" label="Sign in" />
    </div>
  </header>
</template>

<script>
import Icone from "./Icone.vue"
import Button from './Button.vue'
export default {
  components: { Icone, Button }
}
</script>

<style>
  .header {
    display: flex;
    box-sizing: border-box;
    width: 100%;
    height: 8.0rem;
    border-top-right-radius: 20px;
    border-top-left-radius: 20px;
    align-items: center;
    background-color: #000 ;
    padding: 10px 50px;
    justify-content: space-between;
  }
  .header h2 {
    color: #fff;
    margin: 0;
    font-size: 3.0em;
    font-weight: 100;
  }

  .container {
    display: flex;
    align-items: center;
  }

  button {
    margin: 0 5px;
  }

</style>