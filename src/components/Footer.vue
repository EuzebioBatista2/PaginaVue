<template>
  <footer class="container-footer">
    <ul>
      <li class="top">Abstract</li>
      <li><a href="#">Branches</a></li>
    </ul>
    <ul>
      <li class="top">Resources</li>
      <li><a href="#">Blog</a></li>
      <li><a href="#">Help Center</a></li>
      <li><a href="#">Release Notes</a></li>
      <li><a href="#">Status</a></li>
    </ul>
    <ul>
      <li class="top">Community</li>
      <li><a href="#">Twitter</a></li>
      <li><a href="#">Linkedin</a></li>
      <li><a href="#">Facebook</a></li>
      <li><a href="#">Dribbble</a></li>
      <li><a href="#">Podcast</a></li>
    </ul>
    <ul>
      <li class="top">Company</li>
      <li><a href="#">About Us</a></li>
      <li><a href="#">Careers</a></li>
      <li><a href="#">Legal</a></li>
      <li class="Espace"><a href="#">Contact Us</a></li>
      <li><a href="#">Vue@project.com</a></li>
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
      height: 35rem;
      width: 100%;
      border-bottom-right-radius: 20px;
      border-bottom-left-radius: 20px;
      align-items: flex-start;
      justify-content: center;
      background-color: #000 ;
      padding: 2.0rem 5.0rem;
    }

    .top {
      font-size: 2.5rem;
      font-weight: bold;
      margin-bottom: 1.0rem;
      cursor: text;
    }

    ul {
      width: 18%;
      height: 50%;
      list-style: none;
      padding: 0;
      margin: 0;
    }

    .down {
      display: flex;
      flex-direction: column;
      align-items: flex-end;
      justify-content: flex-end;
      width: 28%;
      height: 100%;
    }

    ul li {
      color: #fff;
      font-size: 1.5rem;
      margin-top: 5px;
    }

    ul li a {
      margin-top: 5px;
      text-decoration: none;
      color: #fff;
      font-size: 1.5rem;
    }

    @media(max-width: 960px) {
      .container-footer {
        flex-wrap: wrap;
        height: 50rem;
      }

      ul {
        box-sizing: border-box;
        width: 50%;
        height: 40%;
        padding: 2.0rem;

      }

      .down {
        flex-direction: row;
        height: 20%;
        width: 100%;
        justify-content: flex-start;
        flex-wrap: wrap;
        align-items: center;
      }

      .down .icone {
        margin: 0;
      }

      .down .icone svg {
        height: 20px;
        width: 20px;
      }

      .down li {
        margin: 0;
      }

      .down li::before {
        content: "";
        margin-left: 3px;
        
      }

      .down .icone h1 {
        font-size: 1.5rem;
      }
    }

    @media(max-width: 660px) {
      .container-footer {
        padding: 20px 10px;
      }
      .down {
        align-items: center;
        padding: 0rem;
        padding-left: 2.0rem;
      }
      .down li {
        width: 100%;
      }

    }

</style>