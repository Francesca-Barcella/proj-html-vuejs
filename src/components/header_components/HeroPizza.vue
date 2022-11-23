<script>
import ButtonPrev from '../common_components/ButtonPrev.vue'
import ButtonNext from '../common_components/ButtonNext.vue'

export default {
    name: 'HeroPizza',
    components:{
        ButtonPrev,
        ButtonNext
    }
}
</script>

<template>
    <section class="jumbotron d-flex">
        <ButtonPrev class="prev"/>
        <div class="container d-flex p-2">
            <img src="../../assets/img/h3-rev-img-6.png" alt="">
        </div>
        <ButtonNext class="next"/>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;

.jumbotron{
    justify-content: space-between;
    align-items: center;
    .prev, .next{
        position: relative;
        translate: (0 -50%);
    }
}
.container {
    background-image: url('../../assets/img/h3-rev-img-5.png');
    background-size: contain;
    background-repeat: no-repeat;
    background-position: center;
    height: 500px;
    width: 65%;

    img{
       margin: auto;
    }
}
</style>
