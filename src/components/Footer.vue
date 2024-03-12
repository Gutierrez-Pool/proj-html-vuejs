<script>
export default {
    name: 'Footer',
}
</script>

<template>

    <footer>
        <div class="container">
            <div class="subscribe d-flex justify-content-between">
                <div class="text-white">
                    <h2>We Offer Awesome Services</h2>
                    <p>When, while lovely valley teems with vapour around meand meridian sun strikes the upper surface.</p>
                </div>
                <div>
                    <input type="text">
                </div>
            </div>
    
            <div class="top-footer d-flex justify-content-between">
                <div>
                    logo
                    <p>testo</p>
                </div>
    
                <div>
                    <h6>titolo</h6>
                    <ul>
                        <li>link</li>
                        <li>link</li>
                        <li>link</li>
                    </ul>
                </div>
    
                <div>
                    <h6>titolo</h6>
                    <ul>
                        <li>link</li>
                        <li>link</li>
                        <li>link</li>
                        <li>link</li>
                        <li>link</li>
                    </ul>
                </div>
    
                <div>
                    <h6>titolo</h6>
                    <p>address</p>
                    <p>phone</p>
                    <p>email</p>
                </div>
            </div>

            <div class="bottom-footer d-flex justify-content-between">
                <div>
                    <p>
                        <small>2020 Phlox. All Rights Reserved</small>
                    </p>
                </div>
                <div class="d-flex">
                    <ul class="d-flex gap-5">
                        <li>icon</li>
                        <li>icon</li>
                        <li>icon</li>
                        <li>icon</li>
                    </ul>
                    icon
                </div>
            </div>
        </div>

    </footer>

</template>

<style lang="scss">

footer {
    padding-top: 220px;

    position: relative;
    background-color: #030434;

    .subscribe {
        position: absolute;
        top: -30%;

        width: 1320px;
        
        padding: 95px 45px;
        background: linear-gradient(to right, #b6246e 0%, #f9636b 100%);
        border-radius: 30px;

        h2 {
            font-weight: bold;
            font-size: 42px;
        }
    }

    ul {
        list-style-type: none;
    }

    .bottom-footer {
        ul {
            padding-right: 100px;
        }
    }
}

</style>