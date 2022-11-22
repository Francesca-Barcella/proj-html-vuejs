<script>
export default {
    name: 'TestimonialsSection'
}
</script>

<template>
    <section class="Testimonials">
        <div class="container">
            <img src="" alt="">
            <h3 class="testimonial uppercase py-3">"FORGET THE TRANDY PIZZA SHOP, THIS HIDDEN SPOT MAKES THE BEST NEW
                YORK-STYLE PIZZA SLICE IN NAPPLES"</h3>
            <h5 class="author uppercase pb-3">WASHINGTON POST 2018</h5>
            <div class="d-flex justify-content-center">
                <div class="circle"></div>
                <div class="circle"></div>
                <div class="circle"></div>
            </div>
        </div>
    </section>

</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;

.Testimonials {
    background-color: $proj_bg_ligth;
    background-image: url('../../assets/img/h3-testimonials-bckgrnd.jpg');
    background-size: contain;
    background-repeat: no-repeat;
    background-position: center;
    height: 300px;

    .container {
        justify-content: center;
        text-align: center;
        width: 40%;

        .author {
            color: $proj_primary;
        }

        .circle {
            width: 10px;
            aspect-ratio: 1 / 1;
            border-radius: 50%;
            margin-right: 0.5rem;
            background-color: $proj_secondary;
        }
    }

}
</style>