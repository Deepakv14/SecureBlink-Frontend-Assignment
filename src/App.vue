<template>
<div>
    <DeepakVerma />
    <BannerHead />
    <DataRecords />
    <br />
    <CoursesZone />
    <br/>
    <TopEarner />
    <br/>
    <ReferWork />
    <br/>
    <TestimonialsTab />
    <ContactUs />
    <FooterPart />
</div>
</template>

<script>
import DeepakVerma from './components/DeepakVerma.vue';
import BannerHead from './components/BannerHead.vue';
import DataRecords from './components/DataRecords.vue';
import CoursesZone from './components/CoursesZone.vue';
import TopEarner from './components/TopEarner.vue';
import ReferWork from './components/ReferWork.vue';
import TestimonialsTab from './components/TestimonialsTab.vue';
import ContactUs from './components/ContactUs.vue';
import FooterPart from './components/FooterPart.vue';

export default {
    name: 'App',
    components: {
        DeepakVerma,
        BannerHead,
        DataRecords,
        CoursesZone,
        TopEarner,
        ReferWork,
        TestimonialsTab,
        ContactUs,
        FooterPart,
    }
}
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
}
</style>
