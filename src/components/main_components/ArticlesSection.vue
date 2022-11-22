<script>
export default {
    name: 'ArticlesSection'
}
</script>

<template>
    <section class="articles">
        <div class="container-fluid my-3">
            <div class="row">
                <div class="col"><img src="../../assets/img/h3-img-1.jpg" alt=""></div>
                <div class="col"><img src="../../assets/img/h3-img-2.jpg" alt=""></div>
                <div class="col"><img src="../../assets/img/h3-img-3.jpg" alt=""></div>
                <div class="col"><img src="../../assets/img/h3-img-4.jpg" alt=""></div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;

.row{
    justify-content: space-between;
    /* margin-left: -1.5rem; */
}
.col>img:hover {
    cursor: pointer;
}
</style>