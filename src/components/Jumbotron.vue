<script>
export default {
    name: 'Jumbotron',
}
</script>
<template>
<div class="jumbo">
    <div class="container d-flex justify-content-between align-items-center">
        <div class="col-4 d-flex flex-column">
            <h1>
                <strong>Business Planning</strong>
                Digital Technology
                <strong>Modern Solution !</strong>
            </h1>
            <p>
                <small>
                    When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper surface.
                </small>
            </p>
            <div class="d-flex gap-4">
                <div class="btn red">
                    Try it now
                </div>
                <div class="btn blue">
                    Explore More
                </div>
            </div>
        </div>
        <div class="col-7">
            <img src="/img/header.png" alt="">
        </div>
    </div>
</div>

</template>


<style lang="scss">
@use '../styles/variables' as *;

.jumbo {
    padding: 20px 0px 190px;
    color: white;

    h1 {
        margin-bottom: 45px;
    }

    p {
        margin-bottom: 70px;

        small {
            color: #03a7d3e6;
        }
    }
    
    img {
        width: 100%;
    }

    .btn {
        color: white;
    }

    .btn.red {
        background: linear-gradient(to right, #b6246e 0%, #f9636b 100%);
    }

    .btn.blue {
        background: linear-gradient(to right, #5e7ae8 0%, #05057c 100%);
    }
}


</style>