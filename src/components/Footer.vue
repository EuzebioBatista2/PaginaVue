<template>
  <footer class="container-footer">
    <ul>
      <li class="top">Abstract</li>
      <li>Branches</li>
    </ul>
    <ul>
      <li class="top">Resources</li>
      <li>Blog</li>
      <li>Help Center</li>
      <li>Release Notes</li>
      <li>Status</li>
    </ul>
    <ul>
      <li class="top">Community</li>
      <li>Twitter</li>
      <li>Linkedin</li>
      <li>Facebook</li>
      <li>Dribbble</li>
      <li>Podcast</li>
    </ul>
    <ul>
      <li class="top">Company</li>
      <li>About Us</li>
      <li>Careers</li>
      <li>Legal</li>
      <li class="Espace">Contact Us</li>
      <li>Vue@project.com</li>
    </ul>
    <ul class="down">
      <Icone />
      <li>Copyright 2023</li>
      <li>Desenvolvido por Euzebio</li>
      <li>All rights reserved</li>
    </ul>
  </footer>
</template>

<script>
import Icone from './Icone.vue';
export default {
  name: "Footer",
  components: { Icone }
}
</script>

<style>
    .container-footer {
      display: flex;
      box-sizing: border-box;
      height: 50vh;
      width: 100%;
      border-bottom-right-radius: 20px;
      border-bottom-left-radius: 20px;
      align-items: flex-start;
      justify-content: center;
      background-color: #000 ;
      padding: 2.0rem 7.0rem;
    }

    .top {
      font-size: 2.5rem;
      font-weight: bold;
      margin-bottom: 1.0rem;
      cursor: text;
    }

    ul {
      width: 20%;
      list-style: none;
      padding: 0;
    }

    .down {
      display: flex;
      flex-direction: column;
      align-items: flex-end;
      justify-content: flex-end;
      height: 90%;
    }

    ul.down li {
      cursor: text;
    }

    ul li {
      color: #fff;
      font-size: 1.5rem;
      margin-top: 5px;
      cursor: pointer;
    }

</style>