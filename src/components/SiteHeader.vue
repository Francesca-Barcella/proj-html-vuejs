<script>
import NavBar from './header_components/NavBar.vue'
import HeroPizza from './header_components/HeroPizza.vue'

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
        <NavBar />
        <HeroPizza />
    </header>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables.scss' as *;

header {
    background-color: $proj_dark;
    padding-top:1rem;
    padding-bottom: 2rem;
}
</style>
