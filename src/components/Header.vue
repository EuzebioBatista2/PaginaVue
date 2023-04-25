<template>
  <header class="header">
    <div class="container">
      <Icone />
      <h2>Help center</h2>
    </div>
    <div class="container">
      <Menu />
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
import Menu from './Menu.vue'
export default {
  components: { Icone, Button, Menu }
}
</script>

<style>
  .header {
    display: flex;
    box-sizing: border-box;
    position: relative;
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

  .header h2::before {
    content: "|";
    margin: 0 5px;
  }

  .container {
    display: flex;
    align-items: center;
  }

  button {
    margin: 0 5px;
  }

  div > div.icone:hover svg, div > div.icone:hover h1 {
    fill: #cccccc;
    color: #cccccc;
    cursor: pointer;
  }

  .container .menu {
    display: none;
  }

  @media  (max-width: 960px) {
    .header {
      padding: 5px 25px;
    }
    .container .menu {
      display: flex;
      flex-direction: column;
      width: 20px;
      height: 20px;
      padding: 10px;
      justify-content: space-between;
    }
    .container:nth-child(2) {
      width: 20%;
      justify-content: flex-end;
    }
    .container:nth-child(1) {
      width: 80%;
      justify-content: flex-start;
    }
  }

  @media (max-width: 660px) {
    .header .container{
      flex-direction: column;
      justify-content: center;
      align-items: center;
      flex-wrap: wrap;
    }

    .container h1 {
      font-size: 2.5em ;
    }

    .container h2 {
      font-size: 1.5em ;
    }
    .header h2::before {
      content: "";
      margin: 0 0px;
    }
  }

</style>