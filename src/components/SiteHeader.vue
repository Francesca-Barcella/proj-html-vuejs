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
        <NavBar />
        <HeroPizza />
    </header>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/_variables.scss' as *;

header {
    background-color: $proj_dark;
}
</style>
