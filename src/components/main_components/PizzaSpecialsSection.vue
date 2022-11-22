<script>
export default {
    name: 'PizzaSpecialsSection'
}
</script>

<template>
    <section class="pizza_specials my-2">
        <div class="container-fluid">
            <div class="row">
                <div class="col">IMMAGINE E LOGO</div>
                <div class="col">
                    <h3>prova Pizza Specials Section</h3>
                </div>
            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;
.pizza_specials{
    height: 200px;
    background-color: $proj_secondary;
}
</style>