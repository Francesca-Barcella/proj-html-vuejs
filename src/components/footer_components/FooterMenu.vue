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
        <div class="container-fluid p-2">
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
                        <h6 class="uppercase pe-1">FOLLOW US:</h6>
                        <i class="fa-brands fa-twitter px-2"></i>
                        <i class="fa-brands fa-facebook-f px-2"></i>
                        <i class="fa-brands fa-instagram px-2"></i>
                        <i class="fa-brands fa-linkedin-in px-2"></i>
                    </div>
                </div>
                <!--caption -->
                <div class="col caption uppercase">
                    <div v-for="item in Caption">
                        <h5>{{ item.text }}</h5>
                    </div>
                </div>
                <div class="container-fluid created d-flex">
                    <div>Created with &hearts; by <span>Qode Interactive</span></div>
                    <img src="../../assets/img/h5-logo-divided-header-dark.png" alt="">
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

h6,
h5 {
    color: $proj_secondary;
}

.caption h5 {
    color: $proj_ligth;
}

li {
    color: $proj_dark_ligth;
}

i {
    color: $proj_ligth;
    font-size: smaller;
    transition: 0.5s;

    &:hover {
        color: $proj_secondary;
        cursor: pointer;
    }
}

.created {
    justify-content: space-between;
    align-items: center;

    div {
        align-self: flex-end;
        color: $proj_secondary;
        font-family: 'Noto Sans', sans-serif;
        font-size: small;

        span {
            color: green;
        }
    }

    img {
        max-width: 125px;
    }
}
</style>
