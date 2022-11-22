<script>
export default {
    name: 'OurTeamSection'
}
</script>

<template>
    <section class="our_team">
        <div class="container-fluid my-2">
            <div class="row">
                <div class="col">COL 1 Our Team Section</div>
                <div class="col">COL 2 Our Team Section</div>
                <div class="col">COL 3 Our Team Section</div>
                <div class="col">COL 4 Our Team Section</div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;
.col {
    height: 200px;
    background-color: $proj_primary;
    border: 1px solid black;
}
</style>