<script>
export default {
    name: 'BuildPizzaSection'
}
</script>

<template>
    <section class="build_pizza">
        <div class="container">
            GO AHED ....... DA LAVORARE SULLE IMPOSTAZIONE DEL BACKGROUND SIZE E POSITION
            <h3>prova Build Pizza Section</h3>
        </div>
    </section>

</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;
.build_pizza{
    background-image: url('../../assets/img/h3-background-img.jpg');
    background-size: contain;
    background-repeat: repeat;
    background-position: center;
    height: 385px;
}
</style>