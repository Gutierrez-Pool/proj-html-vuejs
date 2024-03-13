<script>
export default {
    name: 'Pricing',

    data() {
        return {
            pricing: [
                {
                    title: 'Designing',
                    text: 'PROCESS',
                    price: '40',
                    features: [
                        {
                            title: 'Creative',
                            text: 'Design Enabled'
                        },
                        {
                            title: 'Vibrant',
                            text: 'Color Usage'
                        },
                        {
                            title: 'Eye',
                            text: 'Catching Desing'
                        },
                        {
                            title: 'Extreme',
                            text: 'Typography'
                        },
                        {
                            title: 'Exceptional',
                            text: 'Design'
                        },
                    ]
                },
                {
                    title: 'Developing',
                    text: 'PRODUCT',
                    price: '60',
                    features: [
                        {
                            title: 'Creative',
                            text: 'Design Enabled'
                        },
                        {
                            title: 'Vibrant',
                            text: 'Color Usage'
                        },
                        {
                            title: 'Eye',
                            text: 'Catching Desing'
                        },
                        {
                            title: 'Extreme',
                            text: 'Typography'
                        },
                        {
                            title: 'Exceptional',
                            text: 'Design'
                        },
                    ]
                },
                {
                    title: 'Supporting',
                    text: 'CLIENTS',
                    price: '80',
                    features: [
                        {
                            title: 'Creative',
                            text: 'Design Enabled'
                        },
                        {
                            title: 'Vibrant',
                            text: 'Color Usage'
                        },
                        {
                            title: 'Eye',
                            text: 'Catching Desing'
                        },
                        {
                            title: 'Extreme',
                            text: 'Typography'
                        },
                        {
                            title: 'Exceptional',
                            text: 'Design'
                        },
                    ]
                }
            ]
        }
    },
}
</script>

<template>

<div id="pricing">
    <div class="container">
        <h6>Price List</h6>
        <h2><strong>Our</strong> Pricing</h2>
        <p>
            When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper surface.
        </p>

        <div class="d-flex justify-content-around gap-5">
            <div v-for="(price, index) in pricing" class="price-card">
                <span class="bg-prezzo">{{ price.price }}</span>
                <h3><strong>{{ price.title }}</strong></h3>
                <p><small>{{ price.text }}</small></p>
                <div>$</div>
                <span class="prezzo">{{ price.price }}</span>
                <p><small>Per Month</small></p>
                
                <ul>
                    <li v-for="(feature, index) in price.features">
                        <strong>{{ feature.title }}</strong> {{ feature.text }}
                    </li>
                </ul>
                <div class="btn">
                    Order Now
                    <i class="fa-solid fa-arrow-right-long"></i>
                </div>
            </div>
        </div>
    </div>
</div>

</template>

<style lang="scss">

#pricing {
    text-align: center;
    padding-bottom: 165px;

    background: linear-gradient(to bottom, #01012f 0%, #01012f 50%, white 50%, white 100%);
    color: white;

    p {
        padding-bottom: 80px;
    }

    .price-card {
        position: relative;

        background-color: white;
        color: black;

        padding: 55px 80px;
        border-radius: 20px;

        box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);

        .prezzo {
            font-size: 70px;
            font-weight: bold;
        }

        .bg-prezzo {
            position: absolute;
            top: -14%;
            right: -3%;

            font-size: 250px;
            font-weight: bold;

            color: rgba(128, 128, 128, 0.228);
        }

        ul {
            list-style-type: none;
        }

        .btn {
            background: linear-gradient(to bottom, #b6246e 0%, #f9636b 100%);
            color: white;
            padding: 10px 25px;
            border-radius: 30px;
            font-weight: bold;

            i {
                padding-left: 55px;
            }
        }
    }

    .price-card:nth-of-type(2) {
        background: linear-gradient(to bottom, #b6246e 0%, #f9636b 100%);
        color: white;
        box-shadow: none;

        .bg-prezzo {
            color: rgba(255, 255, 255, 0.161);
        }

        .btn {
            background: white;
            color: #f9636b;
        }
    }


}

</style>