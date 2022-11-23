<script>
export default {
    name: 'BookingSection'
}
</script>

<template>
    <section class="booking uppercase mb-2 py-5">
        <form action="book_a_table" class="reservation d-flex">
            <div>
                <input type="text" name="" id="" placeholder="1 person">
            </div>
            <div class="d-flex align-items-center">
                <h4 class="me-3 uppercase">FOR</h4><input type="date" name="" id="">
            </div>
            <div class="d-flex align-items-center">
                <h4 class="me-3 uppercase">AT</h4><input type="time" name="" id="">
            </div>
            <div>
                <input class="submit uppercase" type="submit" value="BOOK A TABLE">
            </div>

        </form>

    </section>

</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;

.booking {
    background-image: url('../../assets/img/h3-background-img-3.jpg');
    background-size: cover;
    background-repeat: no-repeat;

    .reservation{
        max-width: 70%;
        margin: auto;
        justify-content: space-around;
        align-items: center;
    }

    input{
        height: 70px;
        width: 260px;
        border: 1px solid $proj_dark;
        padding: 1rem;
        color: $proj_secondary;
    }
    .submit{
        background-color: $proj_primary;
        color: $proj_ligth;
        border: none;
    }

    h4{
        color: $proj_ligth;
    }
}

</style>