<script>
export default {
    name: 'ClientsSection',
    data() {
        return {
            clients: [
                {
                    url: 'h1-clients-img-1.png'
                },
                {
                    url: 'h1-clients-img-2.png'
                },
                {
                    url: 'h1-clients-img-3.png'
                },
                {
                    url: 'h1-clients-img-4.png'
                },
                {
                    url: 'h1-clients-img-5.png'
                },
            ]
        }
    },
    methods: {
        getImageUrl(name) {
            return new URL(`../../assets/img/${name}`, import.meta.url).href
        }
    }
}
</script>

<template>
    <section class="clients">
        <div class="container py-5">
            <div class="row">
                <div class="col" v-for="item in clients"><img :src=" getImageUrl(item.url)" alt=""></div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;
.clients{
    background-color: $proj_bg_ligth;
}
</style>