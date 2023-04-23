<template>
  <div class="container-card">
    <div class="card">
        <img :src="caminhoSRC" height="40px" width="40px">
        <h1>{{ layout }}</h1>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer hendrerit quis magna et semper. 
            enean pretium est non ex dapibus, non lobortis odio scelerisque. Suspendisse fringilla pharetra 
            libero, nec sollicitudin.
        </p>
        <img class="effect" :src="caminhoSRC" height="280px" width="280px">
    </div>
  </div>
</template>

<script>
export default {
    name: "Card",
    props: {
        layout: {
            type: String,
            required: true
        }
    },
    computed: {
        caminhoSRC() {
            return require(`../assets/bxl-${this.layout}.svg`);
        },
    }

}
</script>

<style>
    .container-card {
        display: flex;
        align-items: center;
        flex-wrap: wrap;
        margin: 40px 10px;
    }

    .card {
        display: flex;
        box-sizing: border-box;
        flex-direction: column;
        position: relative;
        width: 300px;
        align-items: center;
        border: 2px solid #e4e4e4;
        padding: 15px;
        border-radius: 15px;
        cursor: pointer;
        transition: all 0.4s;
        box-shadow: -5px 6px 5px 0px #a09797;
        overflow: hidden;
        
    }

    .card h1 {
        text-transform: uppercase;
    }

    .card p {
        text-align: justify;
        font-weight: 500;
    }

    .card:hover {
        color: #fff;
        background-color: #4f5fd5;
        transform: translateY(-10px);
    }

    .card:hover > img {
        filter: invert(1);
        transition: 0.4s;
    }

    .effect {
        position: absolute;
        opacity: 0.1;
        top: 120px;
        left: 100px;
        align-self: flex-end;
        user-select: none;
        pointer-events: none;
    }

</style>