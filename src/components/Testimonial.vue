<script>
export default {
    name: 'Testimonial',

    data() {
        return {
            testimonials: [
                {
                    img: '/img/szabo-viktor-1266895-unsplash-1024x1024.png',
                    vote: '3',
                    text: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper surface of the impenetrable follage of my trees, and but a thousand',
                    name: 'Michkel Anegl',
                    role: 'Marketing Management'
                },
                {
                    img: '/img/philipe-cavalcante-539505-unsplash-1024x1024.png',
                    vote: '3',
                    text: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper surface of the impenetrable follage of my trees, and but a thousand',
                    name: 'Michkel Anegl',
                    role: 'Marketing Management'
                },
                {
                    img: '/img/fabio-spinelli-695744-unsplash-1024x1024.png',
                    vote: '3',
                    text: 'When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper surface of the impenetrable follage of my trees, and but a thousand',
                    name: 'Michkel Anegl',
                    role: 'Marketing Management'
                },
            ],

            clients: [
                {
                    img: '/img/client-1-1.png'
                },
                {
                    img: '/img/clienty-2.png'
                },
                {
                    img: '/img/clienty-4.png'
                },
                {
                    img: '/img/client-5.png'
                },
                {
                    img: '/img/clienty-3.png'
                },
            ]
        }
    },

    methods: {
        voteStars(currentVote) {
            const fillStars = currentVote;

            const starArray = [];

            for (let i = 0; i < 5; i++) {
                let emptyStars =  'fas fa-star';

                if (i < fillStars) {
                    emptyStars += ' filled';
                }
                starArray.push(emptyStars);
            }
            console.log(fillStars);
            return starArray;
        },
    },
}
</script>

<template>

    <div id="testimonial">
        <div class="container">
            <div class="text-center">
                <h6>Testimonial</h6>
                <h2><strong>What</strong> People Say</h2>
                <p>
                    When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper surface.
                </p>
            </div>

            <div class="review d-flex justify-content-around text-center">
                <div v-for="(testimonial, index) in testimonials" class="col-3">
                    <img :src="testimonial.img" alt=""> <br>
                    <span v-for="emptyStars in voteStars(testimonial.vote)">
                        <i :class="emptyStars"></i>
                    </span>
                    <p>{{ testimonial.text }}</p>
                    <div><strong>{{ testimonial.name }}</strong></div>
                    <div><small>{{ testimonial.role }}</small></div>
                </div>
            </div>

            <div class="clients d-flex justify-content-around align-items-center">
                <div v-for="client in clients">
                    <img :src="client.img" alt="">
                </div>
            </div>
        </div>
    </div>

</template>

<style lang="scss">

#testimonial {

    h6 {
        color: #f9636b;
    }

    .text-center {
        padding-bottom: 125px;
    }

    .review {

        padding-bottom: 190px;
        
        .fas.fa-star {
            margin-bottom: 45px;
            color: gray;
        }

        .fas.fa-star.filled {
            color: #b6246e;
        }

        img {
            width: 110px;

            margin-bottom: 50px;

            border: 5px solid #b6246e;
            border-radius: 50%;
        }
    }

    .clients {
        padding-bottom: 275px;

        img {
            max-width: 145px;
            max-height: 70px;
        }
    }
}

</style>