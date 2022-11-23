<script>
export default {
    name: 'PizzaMenuSection',
    data() {
        return {
            pizzas: [
                {
                    url: 'h3-product-img-1a-100x100.png',
                    name: 'BISMARK',
                    price: '$30.00'
                },
                {
                    url: 'h3-product-img-2a-150x150.png',
                    name: 'FIORI DI ZUCCA',
                    price: '$7.00 - $50.00'
                },
                {
                    url: 'h3-product-img-3a-150x150.png',
                    name: 'VALDOSTANA',
                    price: '$55.00'
                },
                {
                    url: 'h3-product-img-4a-150x150.png',
                    name: 'PIZZA TARTUFATA',
                    price: '$45.00'
                },
                {
                    url: 'h3-product-img-5a-150x150.png',
                    name: 'FRANCESCANA',
                    price: '$25.00'
                },
                {
                    url: 'h3-product-img-6a-100x100.png',
                    name: 'CAMPAGNOLA',
                    price: '$50.00 - $95.00'
                },
            ]
        }
    },
    methods: {
        getImageUrl(name) {
            return new URL(`../../assets/img/${name}`, import.meta.url).href
        }
    }
}
</script>

<template>
    <section class="pizza_menu d-flex flex-column my-2 py-5">
        <!-- descriptio section -->
        <div class="description_section pb-5">
            <h5 class="uppercase pb-3">CHOOSE YOUR FLAVORE</h5>
            <h3 class="uppercase py-1">THE BEST PIZZA MENU IN TOWN</h3>
            <P class="lowercase">Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus reiciendis aliquam
                odit dolores sint
                ipsum ad odio consectetur, quibusdam voluptates itaque numquam dolorem!</P>
        </div>
        <!-- products section -->
        <div class="pizza_card container-fluid pt-5">
            <div class="row">
                <div class="col pizza" v-for="item in pizzas">
                    <img :src="getImageUrl(item.url)" alt="">
                    <h5 class="uppercase pizza_name">{{ item.name }}</h5>
                    <h5 class="uppercase pizza_price">{{ item.price }}</h5>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;

.pizza_menu {
    background-color: $proj_ligth;
    align-items: center;

    .description_section {
        text-align: center;
        width: 40%;

        h5 {
            color: $proj_primary;
        }
    }

    .col.pizza {
        text-align: center;

        img {
            width: 100%;
        }
    }

    .pizza_name {
        color: $proj_secondary;

    }

    .pizza_price {
        color: $proj_primary;
    }
    
    p{
        font-size: 1rem;
    }
}
</style>