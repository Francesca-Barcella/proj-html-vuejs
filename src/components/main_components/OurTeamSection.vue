<script>
export default {
    name: 'OurTeamSection',
}
</script>

<template>
    <section class="our_team">
        <div class="container-fluid my-2">
            <div class="row">
                <div class="col"> </div>
                <div class="col"> </div>
                <div class="col"> </div>
                <div class="col"> </div>
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