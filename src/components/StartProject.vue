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
        
                <div class="d-flex gap-4">
                    <div class="btn red">Try it Now</div>
                    <div class="btn blue">Explore More</div>
                </div>
            </div>
        </div>
    </section>

</template>

<style lang="scss">
@use '../styles/variables' as *;

#start-project {

    padding: 105px 0 150px;
    background: linear-gradient(to top, #01012f 0%, #0b1952 100%);
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

        p {
            color: #03a7d3e6;
        }
    }

    .btn {
        color: white;
        padding: 15px 50px;
        border-radius: 30px;
    }

    .btn.red {
        background: linear-gradient(to right, #b6246e 0%, #f9636b 100%);
    }

    .btn.red:hover {
        background: linear-gradient(to right, #49A0CC 0%, #263C7E 100%);
    }

    .btn.blue {
        background: linear-gradient(to right, #49A0CC 0%, #263C7E 100%);
    }

    .btn.blue:hover {
        background: linear-gradient(to right, #b6246e 0%, #f9636b 100%);
    }
}


</style>