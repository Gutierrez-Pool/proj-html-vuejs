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
                <div class="col-3">
                    <img src="/img/white-logo-2.png" alt="">
                    <p>When, while lovely valley teems with vapour around meand meridian sun strikes the upper impenetrable </p>
                </div>
    
                <div class="col-2">
                    <h6>Quick Links</h6>
                    <ul>
                        <li>Services</li>
                        <li>Contact</li>
                        <li>Blog</li>
                    </ul>
                </div>
    
                <div class="col-2">
                    <h6>Resources</h6>
                    <ul>
                        <li>Art Design</li>
                        <li>Computer</li>
                        <li>IT News</li>
                        <li>Networking</li>
                        <li>Web Security</li>
                    </ul>
                </div>
    
                <div class="col-3">
                    <h6>Contact Us</h6>
                    <p><strong>Address:</strong> Patricia C. Amedee 4401 Waldeck Street Grapevine Nashville Tx 76051</p>
                    <p><strong>Phone:</strong> +99 (0) 101 0000 888</p>
                    <p><strong>Email:</strong> info@yourcomain.com</p>
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
                        <li><i class="fa-brands fa-instagram"></i></li>
                        <li><i class="fa-brands fa-linkedin"></i></li>
                        <li>
                            <i class="fa-brands fa-facebook"></i>
                        </li>
                        <li>
                            <i class="fa-brands fa-twitter"></i>
                        </li>
                    </ul>
                    icon
                </div>
            </div>
        </div>

    </footer>

</template>

<style lang="scss">

footer {
    color: white;
        // test
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

    .top-footer {
        padding-bottom: 110px;

        h6 {
            font-weight: bold;
        }
    }

    .bottom-footer {
        ul {
            padding-right: 100px;
        }
    }
}

</style>