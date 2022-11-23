<script>
export default {
    name: 'ButtonPrev',
}
</script>

<template>

    <div class="prev uppercase">
        <p>PREV</p>
    </div>

</template>

<style lang="scss" scoped>
@use '../../assets/scss/partials/variables.scss' as *;

.prev {
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

.prev>p {
    transform: rotate(+90deg);
}
</style>