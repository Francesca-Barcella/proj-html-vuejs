<script>
export default {
    name: 'ArticlesSection'
}
</script>

<template>
    <section class="articles">
        <div class="container-fluid my-2">
            <div class="row">
                <div class="col">COL 1</div>
                <div class="col">COL 2</div>
                <div class="col">COL 3</div>
                <div class="col">COL 4</div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;
.col{
    height: 200px;
    background-color: $proj_primary;
    border: 1px solid black;
}
</style>