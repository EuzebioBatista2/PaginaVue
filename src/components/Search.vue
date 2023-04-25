<template>
    <div class="search-box">
        <input type="text" class="search-text" placeholder="Pesquisa...">
        <a class="search-btn" href="#">
          <img class='loupe-blue' src="../assets/loupe-blue.svg" width="30px" height="30px">
          <img class='loupe-white' src="../assets/loupe-white.svg" width="30px" height="30px">
        </a>
    </div>
</template>

<script>
export default {

}
</script>

<style>
    .search-box {
        background: #fff;
        height: 5.0rem;
        border-radius: 50px;
        padding: 10px;
        display: flex;
        justify-content: space-between;
        align-items: center;

    }
    .search-text {
        background: none;
        border: 0;
        outline: none;
        font-size: 2.8rem;
        width: 0;

        transition: 0.4s;
    }

    .search-btn {
        width: 5.0rem;
        height: 5.0rem;
        border-radius: 50%;

        display: flex;
        align-items: center;
        justify-content: center;

        cursor: pointer;
    }

    .loupe-white {
        display: none;
    }

    ::-webkit-input-placeholder {
        font-size: 28px;
    }

    .search-box:hover > .search-text {
        width: 450px;
        padding-left: 20px;
    }

    .search-box:hover > .search-btn {
        background: #447ce7;
        transition: 1.0s;
    }

    .search-box:hover > .search-btn .loupe-white {
        display: block;
    }

    .search-box:hover > .search-btn .loupe-blue {
        display: none;
    }

    @media (max-width: 660px) {
        .search-box:hover > .search-text {
            width: 200px;
            padding-left: 20px;
        }
        .display .navigation h1 {
            font-size: 3.5em;
        }

    }

</style>