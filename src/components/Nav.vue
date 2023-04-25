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
        box-sizing: border-box;
        align-items: center;
        flex-direction: column;
        width: 100%;
        padding: 5.0rem 0;
        background-color: #dadbf1;
    }

    .navigation h1 {
        text-align: center;
        font-size: 4.5em;
        margin: 2.0rem 0;
        font-weight: 300;
    }

</style>