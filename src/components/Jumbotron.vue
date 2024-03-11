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
                <div class="btn btn-primary">
                    Try it now
                </div>
                <div class="btn btn-primary">
                    Explore More
                </div>
            </div>
        </div>
        <div class="col-7">
            <img src="/public/img/header.png" alt="">
        </div>
    </div>
</div>

</template>


<style lang="scss">
@use '../styles/variables' as *;

.jumbo {
    padding: 20px 0px 190px;
    background-color: $bg-primary;
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
}


</style>