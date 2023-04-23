<template>
  <nav class="navigation">  
    <h1>How can we help?</h1>
    <Search />

  </nav>
</template>

<script>
import Search from './Search.vue';
export default {
    name: "Nav",
    components: { Search }

}
</script>

<style>
    .navigation {
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        width: 100%;
        height: 350px;
        background-color: #dadbf1;
    }

    .navigation h1 {
        font-size: 4.5em;
        margin: 20px 0;
        font-weight: 300;
    }

</style>