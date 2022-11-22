<script>
export default {
    name: 'HeroPizza'
}
</script>

<template>
    <div class="container d-flex p-2">
        <img src="../../assets/img/h3-rev-img-6.png" alt="">
    </div>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;

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
