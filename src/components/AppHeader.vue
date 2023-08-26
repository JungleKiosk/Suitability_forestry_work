<script>

export default {
    data() {
        return {

        };
    }
}

</script>



<template>
    <header id="goup">
        <div class="container-fluid bg-image">
            <div class="row">
                <div class="col-12 col-lg-12 col-md-8 rounded-4 d-flex align-items-center">
                </div>

                <div class="col-12 col-lg-6 my-5 text-over-bg">
                    <h1 class="title_init m-5 ">Suitability <br> Forestry Work</h1>
                    <h2>
                        This project aims to provide a geospatial analysis-based approach to improve forest planning and
                        forest machine management.<br>
                        Using QGIS as an analysis tool to optimize forest resources in a sustainable way.
                    </h2>
                </div>

            </div>
        </div>
    </header>
</template>
  
<style>
.bg-image {
    height: 800px;
    background-image: url('./../assets/img/ecoservices/eco_header.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat
}

.text-over-bg {
    color: rgb(251, 249, 249);
    background-color: rgba(4, 96, 76, 0.437);
    /* Opacity added to make the text more readable */
    padding: 2rem;
    border-radius: 0 3rem 3rem 0;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

img {
    width: 100%;
}

.title_init {
    font-size: 80px;
    color: #13e764;
}


.logo {
    height: 30px;
    width: auto;
    margin-right: 10px;
}
</style>