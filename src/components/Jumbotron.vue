<script>

export default {
    data() {
        return {

        };
    }
}
</script>



<template>
    <div class="container my-5 txt_jumbo">
        <div class="row justify-content-center ">
            <div class="col-12 col-lg-12">
                <h1 class="title">Stationary Analysis: distance & slope</h1>
                <br>
                <h5>
                    The planning and execution of forestry operations, as well as the passage of forestry machinery, require
                    a careful assessment of the geographical and topographical conditions of the areas concerned.
                    <br> <br>
                    A method in the stationary analysis consists in the analysis of the existing constraints,
                    which could for example prevent forestry operations and therefore exclude the parcel from the Productive
                    Function.
                    <br> <br>
                    Two fundamental variables for the production function are the <span class="title">distance from
                        roads</span> or forest tracks,
                    which can increase costs or even prevent the concentration and extraction of timber, and the <span
                        class="title">slope</span>,
                    which can prevent access to machines and above all significantly increase the risk of erosion.
                    <br> <br>
                    With the <span class="title">Hippoliti and Piegai </span> approach it is possible to evaluate the
                    suitability of the parcels for
                    forestry work through the intersection between the distance from the road and the slope of the forest
                    parcels. This concept is based on the idea that areas with moderate slopes and accessible via existing
                    roads are more suitable for forestry operations and the movement of forestry machinery, while reducing
                    the risk of negative environmental impacts and accidents.
                </h5>
            </div>

            <div class="col-12 col-lg-12 my-5 col-md-8 rounded-4">
                <h2 class="title">LAND SHARING: forest multifunctionality</h2>
                <br>
                <h5>
                    Forests, rich in biodiversity and vitality, offer a wide range of benefits to society and the
                    environment. These benefits,
                    <br>
                    known as <span class="title">ecosystem services</span>, represent the
                    multiple ways in which forest
                    ecosystems contribute to human well-being and ecosystem health. The ecosystem services of forests are
                    closely connected with the various <span class="title">functions</span> that forests perform, such as
                    productive, protective,
                    hydrogeological and recreational functions.
                    <br><br>
                    Applying an accurate system of cuts means <span class="title">maintaining the forest</span> heritage
                    well and making it progress
                    towards a state of greater stability and wealth.
                    All these ecosystem services are provided without any form of remuneration by the forest owner, but now
                    it is one of the central themes of the debate we are witnessing and it is through a payment system for
                    environmental services. <br>
                    The current historical emblem of ecosystem service is the <span class="title">carbon storage</span>, a plant with a diameter of
                    1.2 m and 10 m of height in about 110 years of life has stored around 10 tons of C.
                </h5>

                <div class="row my-5 justify-content-center ">

                    <div class="col-8 col-lg-4 my-5 d-flex align-items-center">
                        <div class="card bg_card card_eco">
                            <h3>Provision Resources</h3>
                            <p>Woods perform a key productive function, providing a wide range of resources. Timber,
                                non-wood
                                products such as fruit, mushrooms and medicinal plants, as well as materials for crafts and
                                industry, form an essential part of the forest's productive services.
                            </p>
                        </div>

                    </div>
                    <div class="col-12 col-lg-6 my-5">
                        <img class="ecoimg_zoom" src="../assets/img/ecoservices/eco_1.jpg" alt="">
                    </div>

                    <div class="col-12 col-lg-6">
                        <img class="ecoimg_zoom" src="../assets/img/ecoservices/eco_2.jpg" alt="">
                    </div>
                    <div class="col-8 col-lg-4 my-5 d-flex align-items-center">
                        <div class="card bg_card card_eco">
                            <h3>Climate Regulation and Microclimate</h3>
                            <p>Forests help regulate global climate through the sequestration of atmospheric carbon and the
                                production of oxygen. Furthermore, they influence the local microclimate, providing shade
                                and
                                cooling the surroundings.
                            </p>
                        </div>

                    </div>

                    <div class="col-4 col-lg-4 my-5 d-flex align-items-center">
                        <div class="card bg_card card_eco">
                            <h3>Recreational Activities</h3>
                            <p>Forests provide spaces for recreation and recreation for
                                people. Outdoor activities such as hiking, cycling, camping and wildlife viewing contribute
                                to
                                people's physical and mental well-being.
                            </p>
                        </div>
                    </div>
                    <div class="col-8 col-lg-6 my-5">
                        <img class="ecoimg_zoom" src="../assets/img/ecoservices/eco_5.jpg" alt="">
                    </div>

                    <div class="col-8 col-lg-6">
                        <img class="ecoimg_zoom" src="../assets/img/ecoservices/eco_4.jpg" alt="">
                    </div>
                    <div class="col-4 col-lg-4 my-5 d-flex align-items-center">
                        <div class="card bg_card card_eco">
                            <h3>Management Water Resources</h3>
                            <p>Forests play a crucial role in regulating the water cycle. They absorb rainwater, reducing
                                the
                                risk of flooding and supplying water to the groundwater. Additionally, tree roots help
                                filter
                                and purify water.
                            </p>
                        </div>

                    </div>

                    <div class="col-8 col-lg-4 my-5 d-flex align-items-center">
                        <div class="card bg_card card_eco">
                            <h3>Protection from Natural Disasters</h3>
                            <p>The protective function of forests is manifested in their ability to mitigate the effects of
                                extreme natural events. Trees act as natural barriers against landslides, floods and
                                avalanches,
                                reducing soil erosion and stabilizing hilly and mountainous areas.
                            </p>
                        </div>

                    </div>
                    <div class="col-12 col-lg-6 my-5">
                        <img class="ecoimg_zoom" src="../assets/img/ecoservices/eco_3.jpg" alt="">
                    </div>





                </div>
            </div>



        </div>
    </div>
</template>




<style scoped>
img {
    width: 100%;
    border-radius: 3rem;
}

.logo_text {
    font-weight: bold;
}

.bg_card {
    background-color: #333333;
    color: white;
    padding: 2rem;
    border-radius: 3rem;
    border: 2px solid #13e764;
}

.ecosystem-services-list {
    list-style: none;
    padding: 0;
}

.service-description {
    font-style: italic;
    font-size: 15px;
    visibility: hidden;
    padding-top: 1rem;
    opacity: 0;
    transition: opacity 0.3s ease, visibility 0.3s ease;
}

.service-description.active {
    visibility: visible;
    opacity: 1;
}

.card_eco {
    transition: transform 0.9s ease;
}

.card_eco:hover {
    transform: scale(1.1);
    background-color: #13e76481;
}

.ecoimg_zoom {
    transition: transform 1.5s ease;
}

.ecoimg_zoom:hover {
    transform: scale(0.9);
}</style>
