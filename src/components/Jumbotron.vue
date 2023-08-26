<script>

export default {
    data() {
        return {

        };
    }
}
</script>



<template>
    <div id="goup" class="container my-5 txt_jumbo">
        <div class="row justify-content-center ">
            <div class="col-12 col-lg-12 col-md-8 bg_item rounded-4">
                <h1 class="title">Wood Functions</h1>
                <p>
                    Forests, rich in biodiversity and vitality, offer a wide range of benefits to society and the
                    environment. These benefits, known as <span class="title">ecosystem services</span>, represent the
                    multiple ways in which forest
                    ecosystems contribute to human well-being and ecosystem health. The ecosystem services of forests are
                    closely connected with the various <span class="title">functions</span> that forests perform, such as
                    productive, protective,
                    hydrogeological and recreational functions.
                </p>

                <div class="row my-5">

                    <div class="col-6 col-lg-6">
                        <h3>Provision Resources</h3>
                        <p>Woods perform a key productive function, providing a wide range of resources. Timber, non-wood
                            products such as fruit, mushrooms and medicinal plants, as well as materials for crafts and
                            industry, form an essential part of the forest's productive services.
                        </p>

                    </div>
                    <div class="col-6 col-lg-6">

                    </div>

                    <div class="col-6 col-lg-6">
                        
                    </div>
                    <div class="col-6 col-lg-6">
                        <h3>Provision Resources</h3>
                        <p>Woods perform a key productive function, providing a wide range of resources. Timber, non-wood
                            products such as fruit, mushrooms and medicinal plants, as well as materials for crafts and
                            industry, form an essential part of the forest's productive services.
                        </p>

                    </div>

                    <div class="col-6 col-lg-6">
                        <h3>Provision Resources</h3>
                        <p>Woods perform a key productive function, providing a wide range of resources. Timber, non-wood
                            products such as fruit, mushrooms and medicinal plants, as well as materials for crafts and
                            industry, form an essential part of the forest's productive services.
                        </p>

                    </div>
                    <div class="col-6 col-lg-6">

                    </div>

                    <div class="col-6 col-lg-6">
                        
                    </div>
                    <div class="col-6 col-lg-6">
                        <h3>Provision Resources</h3>
                        <p>Woods perform a key productive function, providing a wide range of resources. Timber, non-wood
                            products such as fruit, mushrooms and medicinal plants, as well as materials for crafts and
                            industry, form an essential part of the forest's productive services.
                        </p>

                    </div>

                    <div class="col-6 col-lg-6">
                        <h3>Provision Resources</h3>
                        <p>Woods perform a key productive function, providing a wide range of resources. Timber, non-wood
                            products such as fruit, mushrooms and medicinal plants, as well as materials for crafts and
                            industry, form an essential part of the forest's productive services.
                        </p>

                    </div>
                    <div class="col-6 col-lg-6">

                    </div>



                </div>


                <h1 class="title">Stationary Analysis: distance & slope</h1>
                <p>
                    The planning and execution of forestry operations, as well as the passage of forestry machinery, require
                    a careful assessment of the geographical and topographical conditions of the areas concerned.
                    <br>
                    A method in the stationary analysis consists in the analysis of the existing constraints,
                    which could for example prevent forestry operations and therefore exclude the parcel from the Productive
                    Function.
                    <br>
                    Two fundamental variables for the production function are the <span class="title">distance from
                        roads</span> or forest tracks,
                    which can increase costs or even prevent the concentration and extraction of timber, and the <span
                        class="title">slope</span>,
                    which can prevent access to machines and above all significantly increase the risk of erosion.
                </p>
            </div>
        </div>
    </div>
</template>




<style>
.logo_text {
    font-weight: bold;
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

.btn_eco {
    border: 2px solid #13e764;
    color: white;
    background-color: #333333;
    font-weight: bold;
    animation: heartbeat 7s infinite;
}

@keyframes heartbeat {
    0% {
        transform: scale(1);
    }

    25% {
        transform: scale(1.1);
        color: white;
        background-color: #13e76455;
    }
}
</style>
