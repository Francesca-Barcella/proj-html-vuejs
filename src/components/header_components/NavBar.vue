<script>
export default {
    name: 'NavBar'
}
</script>

<template>
    <nav class="navbar p-3">
        <div class="container d-flex">
            <button class="btn_primary p-3" type="submit">ORDER ONLINE</button>
            <!-- left menu -->
            <ul>
                <li class="px-2"><a href="#">HOME</a></li>
                <li class="px-2"><a href="#">PAGES</a></li>
                <li class="px-2"><a href="#">MENU</a></li>
            </ul>
            <!-- brand log -->
            <a class="navbar-brand" href="#"><img src="../../assets/img/h5-logo-divided-header-dark.png" alt=""></a>
            <!-- right menu -->
            <ul>
                <li class="px-2"><a href="#">EVENT</a></li>
                <li class="px-2"><a href="#">BLOG</a></li>
                <li class="px-2"><a href="#">LANDING</a></li>
            </ul>
            <!-- right button -->
            <ul>
                <li class="px-2"><a href="#" class="d-flex"><img class="vespa me-2" src="../assets/svg/svg-1.svg" alt="">CART</a></li>
                <li class="px-2"><a href="#"><img class="vespa me-2" src="../assets/svg/svg-1.svg" alt="">SEARCH</a></li>
            </ul>
        </div>
    </nav>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;

.container {
    justify-content: space-between;
    align-items: center;

    ul {
        display: flex;
        justify-content: space-around;
        align-items: center;
    }

    a {
        font-family: 'Oswald', sans-serif;
        letter-spacing: 0.15rem;
    }

    img {
        width: 160px;
    }

    .vespa {
        width: 35px;
    }

}
</style>
