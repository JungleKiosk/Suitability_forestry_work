<script>

import { marker_points } from "./../data/markers.js";
import AppMap from "./AppMap.vue";

export default {
    components: {
        AppMap
    },
    data() {
        return {
            marker_points: marker_points
        };
    }
}

</script>



<template>
    <div id="goup" class="container my-5 txt_jumbo">
        <div class="row justify-content-center ">
            <div class="col-12 col-lg-12 col-md-8 rounded-4">
                <h1 class="title">Features & History</h1>
                <h5>
                    The main function of the Upper Rabbi forest complex is hydrogeological protection, therefore the
                    productive function plays an entirely secondary role. The strictly economic role is therefore
                    subordinate
                    to social and environmental functions that are not directly quantifiable, but of extremely significant
                    importance ed
                    current. <br> <br>


                    The recreational and environmental tourism functions are already bringing significant economic revenues;
                    wealth not
                    it is therefore provided by the use of forest products but by the ability to offer tourist attractions
                    and services
                    relevant ecosystems. Small quantities of construction timber are also retracted each year or, depending
                    of the improvement interventions carried out, more or less substantial quantities of logs destined
                    to industry (cellulose, cassettes, laminates, etc.). <br> <br>

                    From a management point of view, the Alto Rabbi complex presents a very diversified situation: high
                    forests of conifers, introduced to create artificial reforestation, woods of endemic deciduous trees
                    such as Turkey oak, downy oak, hop hornbeam, maple, beech, shrub species, meadows and pastures that now
                    cover little surface, the latter still testify to the presence of man in these places.<br> <br>

                    Compared to the autochthonous species, conifers have a more rapid growth, even in difficult soils but
                    nevertheless it is
                    it is important to take care of its management, with thinning to limit the unbalanced growth in height
                    and not lead to crashes and weakening of the forest structure, limit the spread of pathogens, the risk
                    of fires and facilitate natural succession and recolonization by endemic species

                    <AppMap :marker_points="marker_points"></AppMap>

                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolor dignissimos, nemo recusandae accusamus,
                    optio ad quasi inventore necessitatibus eos consectetur rerum. Quo repudiandae facere exercitationem
                    cumque soluta, eos qui deleniti! <br>
                </h5>
                <p>
                    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Repellat, deserunt vel. Nam debitis nihil hic
                    quae sit voluptatibus commodi soluta. Assumenda laborum officia quidem nulla ab nobis earum, natus
                    iusto?
                </p>

                <h4 class="text-center">
                    <a href="#goup" style="color: #13e764;">^ Go Up ^</a>
                </h4>
            </div>
        </div>

    </div>
</template>


