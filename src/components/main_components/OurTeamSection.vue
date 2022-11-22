<script>
export default {
    name: 'OurTeamSection',
    data(){
        return{
            teamAvatar:[
                {
                    url: 'h1-team-1a-700x700.jpg'
                },
                {
                    url: 'h1-team-2a.jpg'
                },
                {
                    url: 'h1-team-3a.jpg'
                },
                {
                    url: 'h1-team-4a.jpg'
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
    <section class="our_team">
        <div class="container-fluid my-2">
            <div class="row">
                <div class="col" v-for="item in teamAvatar"><img :src="getImageUrl(item.url)" alt=""></div>

            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;
.col{
    padding: 0;
}
</style>