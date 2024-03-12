<script>
export default {
    name: 'Blog',

    data() {
        return {
            // posts: [
            //     {
            //         date: 'April 21, 2019',
            //         author: 'Paul',
            //         title: 'Amazon gets CCI nod to acquire 49% stake in',
            //         text: 'When, while the lovely valley teems with vapour around meand the meridian sun s ...',
            //         bgImage: '/img/headway-537308-unsplash-1380x703.jpg'
            //     }
            // ]
        }
    },
}
</script>

<template>

    <div id="blog">
        <div class="container">
            <div class="text-center">
                <h6>Blog</h6>
                <h2><strong>Latest</strong> Posts</h2>
                <p>
                    When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper surface.
                </p>
            </div>

            <div class="d-flex justify-content-between">

                <div class="card text-bg-dark col-5">

                    <img src="/img/headway-537308-unsplash-1380x703.jpg" class="card-img" alt="...">
                    
                    <div class="blog-card cardover d-flex ">
                        <div class="">
                            <p class="card-text"><small>April 21, 2019 - by Paul</small></p>
                            <h5 class="card-title">Amazon gets CCI nod to acquire 49% stake in</h5>
                            <p class="card-text">When, while the lovely valley teems with vapour around meand the meridian sun s ...</p>
                        </div>
        
                        <div class="btn btn-light">
                            Read More
                        </div>
                    </div>
                </div>

                <div class="blog-card card col-3">
                    <div class="card-body">
                        <div class="pb-5">
                            <p class="card-text"><small>April 21, 2019 - by Paul</small></p>
                            <h5 class="card-title">Amazon gets CCI nod to acquire 49% stake in</h5>
                            <p class="card-text">When, while the lovely valley teems with vapour around meand the meridian sun s ...</p>
                        </div>
                        <div class="btn btn-light">
                            Read More
                        </div>
                    </div>
                </div>

                <div class="blog-card card col-3">
                    <div class="card-body">
                        <div>
                            <p class="card-text"><small>April 21, 2019 - by Paul</small></p>
                            <h5 class="card-title">Amazon gets CCI nod to acquire 49% stake in</h5>
                            <p class="card-text">When, while the lovely valley teems with vapour around meand the meridian sun s ...</p>
                        </div>
                        <div class="btn btn-light">
                            Read More
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

</template>

<style lang="scss">

#blog {

    padding-bottom: 160px;

    img {
        height: 100%;
    }

    .blog-card {
        padding: 24px 39px;
    
    }
    
    .cardover {
        position: absolute;
        bottom: 0;
        left: 0;
        padding: 40px 55px;
    }
}



</style>