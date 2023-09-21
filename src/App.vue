<script setup>
import MainHeader from './components/MainHeader.vue';
import MainFooter from './components/MainFooter.vue';
import HeroBanner from './components/HeroBanner.vue';
import SponsorBar from './components/SponsorBar.vue';
import SpecialisationSection from './components/SpecialisationSection.vue';
import WorksSection from './components/WorksSection.vue';
import ContactForm from './components/ContactForm.vue';
</script>

<template>
    <MainHeader />

    <!-- Pages -->
    <HeroBanner />
    <SponsorBar />
    <SpecialisationSection />
    <WorksSection />
    <ContactForm />

    <MainFooter />
</template>

<style scoped>

</style>
