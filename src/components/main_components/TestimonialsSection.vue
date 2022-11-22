<script>
export default {
    name: 'TestimonialsSection'
}
</script>

<template>
    <section class="Testimonials">
        <div class="container-fluid">
            <h3>prova Testimonials Section</h3>
        </div>
    </section>

</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;
.Testimonials{
    background-color: $proj_bg_ligth;
    background-image: url('../../assets/img/h3-testimonials-bckgrnd.jpg');
    background-size: contain;
    background-repeat: no-repeat;
    background-position: center;
    height: 300px;

}
</style>