<template>
    <div class="icone">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
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

    .icone svg {
        height: 40px;
        width: 40px;
    }
    .icone h1 {
        color: #fff;
        font-size: 3.0rem;
    }
    @media (max-width: 660px) {
        .icone svg {
            height: 30px;
            width: 30px;
        }
    }


</style>