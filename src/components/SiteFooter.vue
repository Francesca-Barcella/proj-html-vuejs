<script>
import FooterMenu from '../components/footer_components/FooterMenu.vue'
export default {
    name: 'SiteFooter',
    components: {
        FooterMenu
    }
}
</script>

<template>
    <footer id="site-footer">
        <div class="container-fluid">
            <div class="row">
                <div class="col">
                    <FooterMenu />
                </div>
                <div class="col"></div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/_variables.scss' as *;

footer {
    background-color: $proj_dark;
    height: 400px;
    background-image: url('../assets/img/footer-img-1.jpg');
    background-position: right;
    background-repeat: no-repeat;
    background-size: 50%;
}
</style>
