<script>
export default {
    name: 'FooterMenu',
    data() {
        return {
            OurRestaurants: [
                {
                    address: '1614 E. Bell Rd #104',
                    city: 'Salerno, AZ 85022',
                    phone: '(602) 867-1010'
                },
                {
                    address: '204 E. Pizzetta Tommaso',
                    city: 'Sorrento, AZ 85022',
                    phone: '(385) 867-1010'
                },
                {
                    address: 'Vale Puglia 54',
                    city: 'Torre Del Greco Az 85022',
                    phone: '(385) 867-1010'
                },
                {
                    address: 'Corso Italia AA',
                    city: 'Naples, AZ 85022',
                    phone: '(989) 867-1010'
                },
            ],

            WorkingHours: [
                {
                    date: 'MONDAY',
                    hours: 'Kitchen Closed',
                },
                {
                    date: 'TUESDAY UNTIL FRIDAY',
                    hours: '9:00 - 22:00',
                },
                {
                    date: 'SATURDAY',
                    hours: 'Saturday 11am to midnight',
                },
                {
                    date: 'SUNDAY',
                    hours: '9:00 - 22:00',
                },
            ],

            Caption: [
                {
                    text: 'THE DON PEPPE CREW',
                },
                {
                    text: 'FIRST AND FOREMOST',
                },
                {
                    text: 'VALUES AN AUTHENTIC,',
                },
                {
                    text: 'WELL BAKED SLICE OF,',
                },
                {
                    text: 'PIZZA',
                },
            ]
        }
    }
}
</script>

<template>
    <section class="footer_menu">
        <div class="container-fluid top py-2">
            <div class="row py-5">
                <!-- find restaurant -->
                <div class="col">
                    <h5 class="uppercase">FOUND OUR RESTAURANT</h5>
                    <ul class="restaurant py-2 lowercase" v-for="item in OurRestaurants">
                        <li>{{ item.address }}</li>
                        <li>{{ item.city }}</li>
                        <li>{{ item.phone }}</li>
                    </ul>
                </div>
                <!--working hours -->
                <div class="col">
                    <h5 class="uppercase">WORKIN HOURS</h5>
                    <ul class="working_hours py-2" v-for="item in WorkingHours">
                        <li>
                            <h6 class="uppercase">{{ item.date }}</h6>
                        </li>
                        <li class="lowercase">{{ item.hours }}</li>
                    </ul>
                    <div class="social d-flex mt-3">
                        <H6 class="uppercase">FOLLOW US</H6>
                        <i class="fa-brands fa-twitter"></i>
                        <i class="fa-brands fa-facebook-f"></i>
                        <i class="fa-brands fa-instagram"></i>
                        <i class="fa-brands fa-linkedin-in"></i>
                    </div>
                </div>
                <!--caption -->
                <div class="col caption uppercase" >
                    <div v-for="item in Caption">
                        <h5>{{item.text}}</h5>
                    </div>

                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;

.row {
    justify-content: flex-start;
}

.caption h5{
    color: $proj_ligth;
}

</style>
