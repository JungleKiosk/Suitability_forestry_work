<script>
export default {
    data() {
        return {
            showContent: false, // Inizialmente nascondi il contenuto
        };
    },
    methods: {
        toggleContent() {
            this.showContent = !this.showContent; // Inverte lo stato di visualizzazione del contenuto
        },
    },
};
</script>


<template>
    <div class="container my-5 txt_jumbo ">

        <div class="row justify-content-center my-2">
            <div class="col-12 col-lg-6 col-md-6 bg_item_show rounded-4">
                <div class="d-flex align-items-center justify-content-between p-3">
                    <h3 class="title">Flow Chart</h3>
                    <button class="bg_btn mx-3" @click="toggleContent">{{ showContent ? 'Hide' : 'Show' }}</button>
                </div>
                <div v-show="showContent">
                    <p>
                        The first step is to parse the DEM through the GDAL function to process slopes, below
                        the result of processing the raster.
                        <br>
                    <div class="row justify-content-center">

                        <div class="col-12 col-lg-6">
                            <img src="../assets/img/dem.png" alt="">
                        </div>
                        <div class="col-12 col-lg-6">
                            <img src="../assets/img/slope.png" alt="">
                        </div>

                    </div>
                    <br>
                    The second step sees the development of the zonal analysis to obtain the average slopes for each parcel,
                    between the raster just obtained and the vector representing the parcels of the state property complex
                    and also: <br> <br>
                    <ul>
                        <li>Processing > Toolbox > Raster analysis > Zonal statistics > Mean</li>
                    </ul>
                    <br>
                    <div class="row justify-content-center">

                        <div class="col-12 col-lg-6">
                            <img src="../assets/img/slope_mean.png" alt="">
                        </div>

                    </div>
                    <br>
                    The third step is to rate the shape file of the forest roads to create the proximity raster and
                    calculate the average distance from the roads: <br><br>
                    <ol>
                        <li>Create a "logic" field with values equal to 1 in order to have a support variable for the
                            rasterization</li><br>
                        <li>Take the extension of the raster map on the DEM.tif file, specifying it in the
                            Output extent > Use layer extent; as unit we will select pixels and as Width and Height we
                            will indicate the number of columns and rows of the mask
                            raster (2559 and 2630, respectively).</li><br>
                        <li>Raster > Conversion > Rasterize (Vector to raster)</li><br>
                        <li>Processing > Toolbox > Raster analysis > Zonal statistics > Mean</li>
                    </ol>

                    <br>
                    <div class="row justify-content-center">

                        <div class="col-12 col-lg-6">
                            <img src="../assets/img/dist_mean.png" alt="">
                        </div>

                    </div>
                    <br>
                    Finally combine the two single criteria suitability maps together into an overall multi-criteria
                    suitability map, calculating a new Suit_tot field with the Field Calculator as
                    intersection of the two suitability fields for slopes and distance from roads, according to the
                    following logic:
                    <br> <br>
                    <h5 class="text-center">"Suit_slope" AND "Suit_dist"</h5>
                    <div class="row justify-content-center">

                        <div class="col-12 col-lg-6">
                            <img src="../assets/img/suit_and.png" alt="">
                        </div>

                    </div>
                    <br>
                    So to replicate the constraints exposed by the graph of Hippoliti and Piegai, it is necessary to use the
                    boolean operator OR to link the constraints, in order to create the suitability classes the code is as
                    follows:
                    <br> <br>
                    if((( "dist_mean" &lt 1000 ) and ( "slope_mean" &lt 11 )) or (( "dist_mean" &lt 500 ) and ( "slope_mean"
                    &lt 22 )) or (( "dist_mean"&lt 250 ) and ( "slope_mean"&lt 31 )) or (( "dist_mean"&lt 100 ) and (
                    "slope_mean">31 )),1,0)
                    <br> <br>



                    </p>

                    <div class="end_soiltext p-3">
                        <a href="#goup">^ Go Up ^</a>
                        <button class="bg_btn mx-3" @click="toggleContent">{{ showContent ? 'Hide' : '' }}</button>
                    </div>




                </div>
            </div>
        </div>


    </div>
</template>
  

<style>
.end_soiltext a {
    text-decoration: none;
    color: #aaaaaa;
}


.zoom_plots {
    transition: transform 0.2s ease-in-out;
    transform-origin: center center;
}

.zoom_plots:hover {
    transform: scale(1.75);
    border: 0;
}
</style>