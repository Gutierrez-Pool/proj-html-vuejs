<script>
export default {
    name: 'StartProject',
}
</script>

<template>

    <section id="start-project">
        <div class="container d-flex justify-content-around align-items-center">
            <div class="immagini col-4">
                <img id="img-front" src="/img/men-data.png" alt="">
                <img id="img-bg" src="/img/nemoodar.png" alt="">
            </div>
    
            <div class="text col-4 d-flex flex-column">
                <h6>Start Your Project</h6>
                <h1><strong>Grow Your Business</strong> With Our Strategy</h1>
                <p>
                    When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper surface of the impenetrable follage of my trees, and but a few stray gleams steal into the inner sanctuary.
                </p>
        
                <div>
                    <div class="btn btn-danger">Try it Now</div>
                    <div class="btn btn-primary">Explore More</div>
                </div>
            </div>
        </div>
    </section>

</template>

<style lang="scss">
@use '../styles/variables' as *;

#start-project {

    padding: 105px 0 150px;
    background-color: $bg-primary;
    color: white;

    .immagini {
        width: 490px;
        height: 530px;
        position: relative;
    
        img {
            position: absolute;
    
            max-width: 100%;
            max-height: 100%;
        }

        #img-bg {
            max-width: 420px;

            top: -10px;
            left: 10px;
            z-index: 0;
        }

        #img-front {
            max-height: 485px;
            right: 0;
            bottom: 0;
            z-index: 1;
        }
    }

    .text {
        gap: 40px;
    }
}


</style>