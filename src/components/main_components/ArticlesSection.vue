<script>
export default {
    name: 'ArticlesSection',
    data() {
        return {
            imgArticles: [
                {
                    url: 'h3-img-1.jpg'
                },
                {
                    url: 'h3-img-2.jpg'
                },
                {
                    url: 'h3-img-3.jpg'
                },
                {
                    url: 'h3-img-4.jpg'
                }
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
    <section class="articles">
        <div class="container-fluid my-2">
            <div class="row">
                <div class="col" v-for="item in imgArticles"><img :src="getImageUrl(item.url)" alt=""></div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;

.col:first-child, .col:nth-child(2), .col:nth-child(3) {
    margin-right: 0.75rem;
}

.col {
    padding: 0;
    img:hover{
        cursor: pointer;
    }
}

</style>