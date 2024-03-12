<script>
import OurServices from '../components/OurServices.vue';
import StartProject from './StartProject.vue';
import Portfolio from './Portfolio.vue';
import Pricing from './Pricing.vue';
import Blog from './Blog.vue';
import Testimonial from './Testimonial.vue';

export default {
    
    components: {
        OurServices,
        StartProject,
        Portfolio,
        Pricing,
        Blog,
        Testimonial,
    }

}
</script>

<template>
    <OurServices></OurServices>
    <StartProject></StartProject>
    <Portfolio></Portfolio>
    <Pricing></Pricing>
    <Blog></Blog>
    <Testimonial></Testimonial>
</template>

<style></style>