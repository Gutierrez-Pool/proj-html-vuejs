<script>
export default {
    name: 'Pricing',

    data() {
        return {
            pricing: [
                {
                    title: 'Designing',
                    text: 'Process',
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
                    text: 'Product',
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
                    text: 'Clients',
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

        <div class="d-flex justify-content-around">
            <div v-for="(price, index) in pricing" class="price-card col-3">
                <h3>{{ price.title }}</h3>
                <p>{{ price.text }}</p>
                <div>$</div>
                {{ price.price }}
                <p>Per Month</p>
                
                <ul>
                    <li v-for="(feature, index) in price.features">
                        <strong>{{ feature.title }}</strong> {{ feature.text }}
                    </li>
                </ul>
                <div class="btn">
                    Order Now
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

    background-color: #081249;
    color: white;

    .price-card {
        background-color: white;
        color: black;
    }
    ul {
        list-style-type: none;
    }
}

</style>