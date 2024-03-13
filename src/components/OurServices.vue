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
                class="service-card d-flex flex-column"
            >
                <img :src="service.image" alt="">
                <div class="service-text">
                    <h4>{{ service.title }}</h4>
                    <p>{{ service.text }}</p>
                </div>
            </div>
        </div>

        <div class="btn red">
            View All Services
        </div>

    </div>

</template>

<style lang="scss">

#our-services {

    padding: 75px 0px 100px;
    text-align: center;

    .title {
        padding-bottom: 140px;

        h6 {
            color: #F9636B;
        }
    }

    .service {
        padding-bottom: 215px;

        .service-card {
            position: relative;

            width: calc(100% / 4);

            img {
                position: absolute;
                top: -130px;
                left: 80px;
                z-index: 1;

                width: 240px;
                height: 240px;

                padding: 50px 35px;
                background-color: white;
                border-radius: 30px;
            }

            .service-text {
                width: 400px;

                padding: 160px 80px 70px;
                border-radius: 30px;
                color: black;
            }
        
            h4 {
                padding-bottom: 30px;
            }
        }

    }

    .service-card:hover {

        img {
            box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
        }
        
        .service-text {
            color: white;
            background: linear-gradient(to top, #01012f 0%, #1e3db8 100%);
        }

    }

    .btn.red {
        color: white;
        padding: 15px 50px;
        border-radius: 30px;
        background: linear-gradient(to right, #b6246e 0%, #f9636b 100%);
    }

    .btn.red:hover {
        box-shadow: 0px 3px 8px 1px #f9636b, 0 6px 20px 0 rgba(238, 204, 204, 0.19);
    }

}


</style>