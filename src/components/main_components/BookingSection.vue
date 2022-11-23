<script>
export default {
    name: 'BookingSection'
}
</script>

<template>
    <section class="booking uppercase mb-2">
        <h2>INSERIRE FORM PER BOOKIGN</h2>
        <form action="book_a_table">ciao</form>

    </section>

</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;

.booking {
    background-image: url('../../assets/img/h3-background-img-3.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    height: 190px;
}
</style>