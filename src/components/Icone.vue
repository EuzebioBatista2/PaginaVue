<template>
    <div class="icone">
        <svg xmlns="http://www.w3.org/2000/svg" :width="medium" :height="medium" viewBox="0 0 24 24">
          <path d="m12 12.765 5.592-9.437h-3.276L12 7.33v.002L9.688 3.328h-3.28z" />
          <path d="M18.461 3.332 12 14.235 5.539 3.332H1.992L12 20.672l10.008-17.34z" />
        </svg>
        <h1>Projeto Vue</h1>
    </div>
</template>

<script>
export default {
    name: 'Icone',
    data: function() {
        return {
            medium: '40',
        }
    }
    

}
</script>

<style>
    .icone {
        fill: #fff;
        height: 40px;
        display: flex;
        align-items: center;
        
    }
    .icone h1 {
        color: #fff;
        font-size: 1.5em;
    }
    .icone:hover svg, .icone:hover h1 {
        fill: #cccccc;
        color: #cccccc;
        cursor: pointer;
    }

    

</style>