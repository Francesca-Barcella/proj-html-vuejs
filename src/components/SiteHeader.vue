<script>
import NavBar from './NavBar.vue'
import HeroPizza from './HeroPizza.vue'


export default {
    name: 'SiteHeader',
     components: {
        NavBar,
        HeroPizza
     }
}
</script>

<template>
    <header id="site-header">
        <div class="container">
            <NavBar />
            <HeroPizza />
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/_variables.scss' as *;

header {
    background-color: $proj_dark;
    .container {
        background-image: url('../assets/img/h3-rev-img-5.png');
        background-size: contain;
        background-repeat: no-repeat;
        background-position: center;
        height: 500px;
        width: 50%;
    }
}
</style>
