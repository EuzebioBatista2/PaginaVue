<template>
  <div>
    <div class="menu" id="teste" @click="evento">
      <span></span>
      <span></span>
      <span></span>
    </div>
    <div id="content-menu">
      <a href="#"><h1>Submit a request</h1></a>
      <a href="#"><h1>Sign in</h1></a>
    </div>
  </div>
</template>

<script>
import Button from './Button.vue'
export default {
  methods: {
    evento() {
      const menu = document.getElementById("content-menu")
      menu.classList.toggle('evento')

      const menuLink = document.getElementById("teste")
      menuLink.classList.toggle('active')
    },
    components: { Button }
  }

}
</script>

<style>
    .menu {
      display: flex;
      flex-direction: column;
      width: 20px;
      height: 20px;
      background-color: transparent;
      padding: 10px;
      justify-content: space-between;
      cursor: pointer;
    }

    #content-menu {
      display: block;
      position: absolute;
      overflow: hidden;
      left: 0;
      top: 8.0rem;
      box-sizing: border-box;
      background-color: #000000d3;
      width: 100%;
      height: 0;
      transition: 0.4s;
    }

    #content-menu h1 {
      display: flex;
      align-items: center;
      width: 100%;
      box-sizing: border-box;
      height: 7.0rem;
      padding: 1.0rem;
      margin: 0;
      transition: 0.4s;
    }

    #content-menu a h1 {
      display: flex;
      
      align-items: center;
      outline: none;
      width: 100%;
      color: #fff;
    }
    #content-menu a {
      display: block;
      text-decoration: none;
      margin: 1.0rem 3.0rem;
    }

    #content-menu a h1:hover {
      background-color: #4f5fd5;
      border-radius: 5px;
      border: 0px solid #fff;
    }

    #content-menu.evento {
      display: block;
      height: 26.5rem;
    }

    .active.menu span:nth-child(1) {
      transform: translateY(9px) rotate(-45deg);
      background-color: red;
    }

    .active.menu span:nth-child(2) {
      width: 0;
    }

    .active.menu span:nth-child(3) {
      transform: translateY(-9px) rotate(45deg);
      background-color: red;
    }

    .menu span {
      height: 2px;
      width: 100%;
      transition: all 0.4s;
      background-color: #fff;
    }

</style>