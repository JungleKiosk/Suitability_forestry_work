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
        <div class="container p-4">
            <div class="row justify-content-center">
                <div class="col-12 col-lg-8 col-md-8 rounded-4 d-flex align-items-center justify-content-center">
                    <h1 class="title text-center p-2">Materials & Methods</h1>
                </div>
            </div>
        </div>

        <div class="row justify-content-center my-2">
            <div class="col-12 col-lg-6 col-md-6 bg_item_show rounded-4">
                <div class="d-flex align-items-center justify-content-between p-3">
                    <h3 class="title">Constraint treatment</h3>
                    <button class="bg_btn mx-3" @click="toggleContent">{{ showContent ? 'Hide' : 'Show' }}</button>
                </div>
                <div v-show="showContent">
                    <p>
                        The objective is to classify the parcels according to these criteria in order to identify those
                        areas that could be used productively and sustainably for activities related to forest management.
                        <br> <br>
                        The fundamental criteria, the slope and the distance from the roads, are considered without any
                        mutual compensation. In other words, one suitable criterion cannot compensate for the lack of
                        suitability of the other criterion.
                        <br><br>
                        The GIS analysis procedure is based on the concept of <span class="title">Boolean
                            intersection</span> of the constraints
                        placed. In essence, it overlays slope and road distance information onto a geospatial map, allowing
                        you to locate parcels that meet the requirements specified by both criteria.
                        <br><br>
                        Within the scheme proposed by <span class="title">Hippoliti and Piegai</span>, different intervals
                        of distance from the roads
                        and slope are defined which influence the suitability of the parcels. These intervals are:

                    <ul>
                        <li>Distance from roads &lt; 1000m, slope &lt; 20%</li>
                        <li>Distance from roads &lt; 500m, 20% &lt; slope &lt; 40%</li>
                        <li>Distance from roads &lt; 250m, 40% &lt; slope &lt; 60%</li>
                        <li>Distance from roads &lt; 100m, slope &gt; 60%</li>
                    </ul>
                    <img class="rounded-4" src="../assets/img/graph_hippieg.png" alt="">

                    <br> <br> <br>

                    To define the suitability for the slope, an average of <span class="title">70% is set as the acceptable
                        limit, equivalent to
                        a 35° slope</span>; it is intended to limit the journey to forestry machinery.
                    To do this, it is possible to exploit a raster <span class="title">DEM</span> to create a map of the
                    slopes and calculate the
                    average of the values of all the pixels falling within the parcels.
                    <br> <br>
                    An important consideration is that if there are parcels with an average distance from the roads of less
                    than 100m, only a portion of the aforementioned will actually be suitable but since the parcel is the
                    fundamental management unit, it is unthinkable to attribute station suitability to it; alternatively you
                    could subdivide the
                    particle into two subparticles.
                    <br> <br>
                    Slopes greater than 60% imply the impossibility of transit of forestry work machines, therefore an
                    accumulation of timber on the road using the winch.
                    <br> <br> <br>

                    <img class="rounded-4" src="../assets/img/winch_forest.png" alt="">

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