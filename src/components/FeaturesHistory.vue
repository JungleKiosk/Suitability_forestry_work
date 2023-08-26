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

                    With an area of about 5000ha, the Alto Rabbi complex is part of the land belonging to the
                    forestry-forestry property of the Emilia-Romagna Region, managed by the Provincial Administration of
                    Forlì-Cesena.
                    The entire area falls entirely within the Municipality of Premilcuore, defining the Tuscan-Emilian
                    border along the ridge. <br> <br>

                    The orography is very articulated, between the ridges that reach altitudes between 700 and 900 m a.s.l.;
                    the data more
                    interesting to analyze in the development of an adjustment plan are however the exposure and slope, i
                    which can strongly influence the usability of the place. In practice, high slope values can
                    make the mechanization of interventions in the forest more difficult and accentuate the hydrogeological
                    risk,
                    while the exposure will have an effect on the potential of the tourist-recreational function
                    <br> <br>
                    The property falls largely within the Foreste Casentinesi National Park, it is included in large part
                    part in the Protection Zones C which include areas of great landscape and natural interest, where the
                    forest management is carried out according to "multifunctional" cultivation models, capable of carrying
                    out jointly
                    functions of environmental, naturalistic, productive, economic and social protection; only to a small
                    extent does it touch some
                    Zone B corresponding to areas which should not be affected by other activities than those aimed at
                    forestry or extensive agricultural management. Furthermore, the SCI/SPA IT4080003 “Monte Gemelli, Monte
                    Guffone”, with large areas falling within priority zones, which impose legislative constraints
                    operating.<br> <br>
                    These last considerations, very important from a design point of view, will not however be considered
                    during the study
                    development of the settlement plan, as announced in the introduction.
                    <br> <br>
                    The plant composition is diversified among a large number of forest species, in particular, are observed
                    endemic hardwood forests, among which the presence of beech and black hornbeam is particularly
                    important, the
                    which are currently managed with coppice on high slopes and tall trees on smaller slopes; high forests
                    of
                    conifers, mainly represented by black pine and spruce, widely used in past years for
                    carry out artificial reforestation due to their rapid development capacity. Indeed, from the historical
                    record, yes
                    deduces how over the years the land use has changed both from an environmental and cultural point of
                    view
                    and social.
                    <br> <br>
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


                </h5>

                <h4 class="text-center">
                    <a href="#goup" style="color: #13e764;">^ Go Up ^</a>
                </h4>
            </div>
        </div>

    </div>
</template>


