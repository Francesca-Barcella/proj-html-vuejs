<script>
import ArticlesSection from './main_components/ArticlesSection.vue';
import TestimonialsSection from './main_components/TestimonialsSection.vue';
import PizzaSpecialsSection from './main_components/PizzaSpecialsSection.vue';
import BuildPizzaSection from './main_components/BuildPizzaSection.vue';
import OurTeamSection from './main_components/OurTeamSection.vue';
import ClientsSection from './main_components/ClientsSection.vue';
import PizzaMenuSection from './main_components/PizzaMenuSection.vue';
import PizzaDealsSection from './main_components/PizzaDealsSection.vue';
import BookingSection from './main_components/BookingSection.vue';


export default {
    name: 'SiteMain',
    components: {
        ArticlesSection,
        TestimonialsSection,
        PizzaSpecialsSection,
        BuildPizzaSection,
        OurTeamSection,
        ClientsSection,
        PizzaMenuSection,
        PizzaDealsSection,
        BookingSection,
    }
}
</script>

<template>
    <main id="site-main">
        <ArticlesSection />
        <TestimonialsSection />
        <PizzaSpecialsSection />
        <BuildPizzaSection />
        <OurTeamSection />
        <ClientsSection />
        <PizzaMenuSection />
        <PizzaDealsSection />
        <BookingSection />
    </main>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/_variables.scss' as *;
</style>
