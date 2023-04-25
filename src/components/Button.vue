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
    button {
        color: #dadbf1;
        border-radius: 10px;
        padding: 10px 30px;
        font-size: 2.0rem;
        cursor: pointer;
    }
    .black {
        background-color: #191b1d;
        border: 1px solid #dadbf1;
        
    }

    .white {
        background-color: #4f5fd5;
        border: none;
        transition: 0.4s;
    }

    .white:hover {
        background-color: #dadbf1;
        color: #191b1d;
    }

    @media (max-width: 960px) {
        button {
            display: none;
        }
    }

</style>