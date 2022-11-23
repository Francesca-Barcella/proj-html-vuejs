<script>
export default {
    name: 'PizzaSpecialsSection'
}
</script>

<template>
    <section class="pizza_specials my-2">
        <div class="container-fluid">
            <div class="row">
                <div class="col persons d-flex py-2"><img src="../../assets/img/h1-img-7n.png" alt=""></div>
                <div class="col menu">
                    <h3>prova Pizza Specials Section</h3>
                </div>
            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;
.pizza_specials{

    background-color: $proj_secondary;

    .persons{
        background-image: url(../../assets/img/h1-img-4.jpg);
        background-size: cover;
        background-repeat: no-repeat;
        justify-content: center;
    }
}
</style>