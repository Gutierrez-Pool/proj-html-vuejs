<script>
export default {
    name: 'Navbar',

    data() {
        return {
            links: [
                'Home', 'About', 'Services', 'Blog', 'Contact', 'Portfolio'
            ],

            activeLink: '0',
        }
    },
}
</script>


<template>

<nav>
    <div class="container">
        <div class="d-flex justify-content-between align-items-center">
            <img src="/img/white-logo-2.png" alt="logo">

            <div class="d-flex align-items-center gap-5">
                
                <ul class="links">
                    <li
                        v-for="(link, index) in links"
                        :class="index == activeLink ? 'active' : ''"
                    >
                       {{ link }} 
                    </li>
                </ul>
        
                <div class="btn">
                    Sign In
                </div>
            </div>
    
        </div>
    </div>
</nav>

</template>


<style lang="scss">
@use '../styles/variables' as *;

nav {
    padding: 20px 0;
    // background-color: $bg-primary;
    color: white;

    img {
        height: 55px;
    }

    ul {
        display: flex;
        
        margin-bottom: 0;
        list-style-type: none;
        gap: 30px;

        li {
            &.active {
                color: #F9636B;
                font-weight: bold;
            }
        }

    }

    .btn {
        color: white;
        background: linear-gradient(to right, #5e7ae8 0%, #05057c 100%);

    }
}
</style>