<script>
export default {
    name: 'PizzaDealsSection'
}
</script>

<template>
    <section class="pizza_deals my-2">
        <div class="container-fluid">
            <div class="row">
                <div class="col">LISTA DEALS</div>
                <div class="col">IMMAGINE DI SFONDO</div>
            </div>
        </div>

    </section>

</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;

.pizza_deals {
    background-color: $proj_secondary;
    height: 300px;
}
</style>