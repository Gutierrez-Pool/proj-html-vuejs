<script>
export default {
    name: 'OurServices',

    data() {
        return {
            services: [
                {
                    image: '/img/Group-247.png',
                    title: 'Data Analysis',
                    text: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper'
                },
                {
                    image: '/img/Group-567.png',
                    title: 'SEO Optimization',
                    text: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper'
                },
                {
                    image: '/img/Group-538.png',
                    title: 'Security Data',
                    text: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper'
                },
                {
                    image: '/img/Group-566.png',
                    title: 'Branding Strategy',
                    text: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper'
                },
            ]
        }
    },
}
</script>

<template>

    <div id="our-services" class="container">
        <div class="title">
            <h6>Our Services</h6>
            <h2><strong>What</strong> We Do</h2>
            <p>When, while the lovely valley teems with vapour around meand the</p>
        </div>

        <div class="service d-flex justify-content-around align-items-center">
            <div 
                v-for="service in services"
                class="col-2 d-flex flex-column"
            >
                <img :src="service.image" alt="">
                <h4>{{ service.title }}</h4>
                <p>{{ service.text }}</p>
            </div>
        </div>

        <div class="btn btn-danger">
            View All Services
        </div>

    </div>

</template>

<style>

#our-services {

    padding: 75px 0px 100px;
    text-align: center;

    .title {
        padding-bottom: 140px;
    }

    .service {
        padding-bottom: 215px;

        img {
            width: 100%;
            max-height: 250px;
            padding-bottom: 65px;
        }
    
        h4 {
            padding-bottom: 30px;
        }
    }

}


</style>