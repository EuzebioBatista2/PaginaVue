<template>
  <button>{{ label }}</button>
</template>

<script>
export default {
    name: "Button",
    props: {
        label: {}
    }

}
</script>

<style>
    .black {
        background-color: #191b1d;
        border: 1px solid #dadbf1;
        color: #dadbf1;
        border-radius: 10px;
        padding: 10px 30px;
        font-size: 1.5em;
        cursor: pointer;
    }

    .white {
        background-color: #4f5fd5;
        border: none;
        color: #dadbf1;
        border-radius: 10px;
        padding: 10px 30px;
        font-size: 1.5em;
        cursor: pointer;
        transition: 0.4s;
    }

    .white:hover {
        background-color: #dadbf1;
        color: #191b1d;
    }

</style>