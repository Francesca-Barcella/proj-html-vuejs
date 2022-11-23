<script>
export default {
    name: 'TestimonialsSection'
}
</script>

<template>
    <section class="Testimonials">
        <div class="container_testimonials d-flex">
            <!-- button prev -->
            <div class="prev uppercase">
                <p>PREV</p>
            </div>
            <!-- testimonial review -->
            <div class="reviews">
                <i class="fa-sharp fa-solid fa-quote-left pt-5 quote"></i>
                <h2 class="uppercase py-1">"FORGET THE TRANDY PIZZA SHOP, THIS HIDDEN SPOT MAKES THE BEST
                    NEW
                    YORK-STYLE PIZZA SLICE IN NAPPLES"</h2>
                <h5 class="author uppercase pb-3">WASHINGTON POST 2018</h5>
                <div class="d-flex justify-content-center pb-5">
                    <div class="circle"></div>
                    <div class="circle"></div>
                    <div class="circle"></div>
                </div>
            </div>
            <!-- button next -->
            <div class="next uppercase">
                <p>NEXT</p>
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

    .container_testimonials{
        justify-content: space-between;
        align-items: center;
    }

    .prev,
    .next {
        background-color: $proj_ligther;
        color: $proj_primary;
        font-size: 15px;
        font-weight: bold;
        width: 100px;
        height: 100px;
        display: flex;
        align-items: center;
        justify-content: start;
        shape-outside: circle(50% at 30%);
        //il primo valore indica quanto tagliare il cerchio e il secondo la posizione del centro del cerchio
        clip-path: circle(50% at 2%);
    }

    .next {
        transform: rotate(-180deg);
    }

    .prev>p,
    .next>p {
        transform: rotate(+90deg);
    }

    .reviews {
        justify-content: space-evenly;
        text-align: center;
        width: 40%;

        .quote {
            color: $proj_secondary;
            font-size: 60px;
        }

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