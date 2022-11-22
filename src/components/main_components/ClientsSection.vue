<script>
export default {
    name: 'ClientsSection'
}
</script>

<template>
    <section class="clients">
        <div class="container">
            <div class="row">
                <div class="col">client 1</div>
                <div class="col">client 2</div>
                <div class="col">client 3</div>
                <div class="col">client 4</div>
                <div class="col">client 5</div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;

.col{
    border: 1px solid red;
    height: 190px;
}
</style>