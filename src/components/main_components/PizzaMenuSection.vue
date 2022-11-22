<script>
export default {
    name: 'PizzaMenuSection'
}
</script>

<template>
    <section class="pizza_menu my-2">
        <div class="container-fluid">
            <div class="description">bla bla bla</div>
            <div class="row">
                <div class="col">pizza 1</div>
                <div class="col">pizza 2</div>
                <div class="col">pizza 3</div>
                <div class="col">pizza 4</div>
                <div class="col">pizza 5</div>
                <div class="col">pizza 6</div>
            </div>
        </div>
    </section>

</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;
.pizza_menu{
    background-color: $proj_primary_ligth;
    height: 550px;
}
</style>