<script>
export default {
    name: 'PizzaDealsSection',
    data() {
        return {
            pizzaDeals: [
                {
                    date: '02',
                    month: 'NOV',
                    event: 'TRADITIONAL NEAPOLITAN PIES IN KYOTO PIZZA MERCATO',
                    address: '204 E. Pizzetta Tommaso.'
                },
                {
                    date: '03',
                    month: 'NOV',
                    event: 'TERRAZZA PATIO DINING SPACE OPENING THI WEEKEND',
                    address: '204 E. Pizzetta Tommaso.'
                },
                {
                    date: '05',
                    month: 'NOV',
                    event: 'SIENNA PRIBìVATE DINING ROOM WITH STEPHANE BRUNN',
                    address: '204 E. Pizzetta Tommaso.'
                },
            ]
        }
    }
}
</script>

<template>
    <!-- ATTENZIONE! QUI STAO USANDO IL FLEX ROW-REVERSE!!! -->
    <section class="pizza_deals my-2">
        <div class="container-fluid">
            <div class="row flex-row-reverse">
                <!-- right* section image -->
                <div class="col comic_strip d-flex"><img src="../../assets/img/h3-img-5a.jpg" alt=""></div>
                <!-- left* section pizza deals -->
                <div class="col deals d-flex py-5">
                    <div class="deal_card py-3">
                        <!--data deal -->
                        <div class="title pb-5">
                            <h6 class="uppercase pb-1">MADE WITH LOVE</h6>
                            <h2 class="uppercase">DELISH PIZZA DEALS</h2>
                        </div>
                        <!-- dettagli deal -->
                        <div class="event_details d-flex py-2 pt-2" v-for="item in pizzaDeals">
                            <div class="event_date uppercase pe-4 flex-column">
                                <h2 class="uppercase">{{ item.date }}</h2>
                                <h4 class="uppercase px-2">{{ item.month }}</h4>
                            </div>
                            <div class="event_name pb-4 pt-2">
                                <h3 class="uppercase">{{ item.event }}</h3>
                                <p class="lowercase pt-1"><i class="fa-solid fa-location-dot me-2"></i>{{ item.address
                                }}
                                </p>
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

.pizza_deals {
    background-color: $proj_dark;

    .deals {
        justify-content: center;
    }

    .deal_card {
        width: 50%;
    }

    .event_details:nth-child(2),
    .event_details:nth-child(3) {
        border-bottom: 1px dashed $proj_secondary;
    }

    h6,
    .event_details h2,
    .event_name p {
        color: $proj_primary;
    }

    .title>h2,
    .event_details h4,
    h3 {
        color: $proj_ligth;
    }
 
    .event_details h2{
        font-size: 45px;
    }
}
</style>