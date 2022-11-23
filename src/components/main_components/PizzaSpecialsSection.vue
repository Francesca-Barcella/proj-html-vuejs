<script>
export default {
    name: 'PizzaSpecialsSection',
    data() {
        return {
            comboMenu: [
                {
                    price: '$10',
                    name: 'COMBO PICCOLO',
                    descritption: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit.'
                },
                {
                    price: '$20',
                    name: 'COMBO MEZZO',
                    descritption: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit.'
                },
                {
                    price: '$30',
                    name: 'COMBO GRANDE',
                    descritption: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit.'
                },
            ]
        }
    }
}
</script>

<template>
    <section class="pizza_specials my-2">
        <div class="container-fluid">
            <div class="row">
                <!-- rigth section image & logo -->
                <div class="col persons d-flex py-5"><img src="../../assets/img/h1-img-7n.png" alt=""></div>
                <!-- left section specials menu -->
                <div class="col specials d-flex py-5">
                    <div class="menu py-3">
                        <!--title section specials menu -->
                        <div class="description pb-3">
                            <h2 class="uppercase pb-1">SPECIALS*</h2>
                            <p class="lowercase">Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore quod a
                                soluta distinctio?</p>
                        </div>
                        <!-- list specials menu -->
                        <div class="cards_menu d-flex py-2" v-for="item in comboMenu">
                            <div class="price uppercase p-1">
                                <h4 class="uppercase">{{item.price}}</h4>
                            </div>
                            <div class="card_menu p-1">
                                <h4 class="uppercase">{{item.name}}</h4>
                                <p class="lowercase pt-1">{{item.descritption}}</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;

.pizza_specials {
    .persons {
        background-image: url(../../assets/img/h1-img-4.jpg);
        background-size: cover;
        background-repeat: no-repeat;
        justify-content: center;
    }

    .specials {
        justify-content: center;
    }

    .menu {
        flex-direction: column;
        align-items: center;
        width: 50%;
    }

    p {
        color: $proj_dark_ligth;
        letter-spacing: 0.1rem;
        font-size: 1rem;
    }

    .price>h4 {
        color: $proj_primary;
    }
}
</style>