<script>
export default {
    name: 'BuildPizzaSection'
}
</script>

<template>
    <section class="build_pizza">
        <div class="container uppercase py-5">
            GO AHEAD AND <br>
            BUILD YOUR <br>
            OWN PIZZA <br>
            WE WON'T <br>
            JUDGE! <br>
        </div>
    </section>

</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;

.build_pizza {
    background-image: url('../../assets/img/h3-background-img.jpg');
    background-size: contain;
    background-repeat: repeat;
    background-position: center;
    font-size: 70px;
    font-weight: bold;
    color: $proj_ligth;
}
</style>