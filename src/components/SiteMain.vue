<script>
import ArticlesSection from './main_components/ArticlesSection.vue';
import ReviewsSection from './main_components/ReviewsSection.vue';
import PizzaSpecialsSection from './main_components/PizzaSpecialsSection.vue';
import BuildPizzaSection from './main_components/BuildPizzaSection.vue';
import OurTeamSection from './main_components/OurTeamSection.vue';
import PizzaMenuSection from './main_components/PizzaMenuSection.vue';
import PizzaDealsSection from './main_components/PizzaDealsSection.vue';
import BookingSection from './main_components/BookingSection.vue';



export default {
    name: 'SiteMain',
    components: {
        ArticlesSection,
        ReviewsSection,
        PizzaSpecialsSection,
        BuildPizzaSection,
        OurTeamSection,
        PizzaMenuSection,
        PizzaDealsSection,
        BookingSection
    }
}
</script>

<template>
    <main id="site-main">
        <ArticlesSection />
        <ReviewsSection />
        <PizzaSpecialsSection />
        <BuildPizzaSection />
        <OurTeamSection />
        <PizzaMenuSection />
        <PizzaDealsSection />
        <BookingSection />
    </main>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/_variables.scss' as *;
</style>
