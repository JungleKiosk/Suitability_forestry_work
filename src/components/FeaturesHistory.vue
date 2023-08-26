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
            <div class="col-12 col-lg-12 col-md-8 bg_item rounded-4">
                <h1>Features & History</h1>
                <p>
                    Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ipsum, aut! Debitis qui possimus ipsum, velit
                    eum fuga iusto accusantium cum eaque delectus laborum, nisi aut ut excepturi, aspernatur dolorum
                    impedit!

                    <AppMap :marker_points="marker_points"></AppMap>

                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolor dignissimos, nemo recusandae accusamus,
                    optio ad quasi inventore necessitatibus eos consectetur rerum. Quo repudiandae facere exercitationem
                    cumque soluta, eos qui deleniti! <br>
                </p>
                <p>
                    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Repellat, deserunt vel. Nam debitis nihil hic
                    quae sit voluptatibus commodi soluta. Assumenda laborum officia quidem nulla ab nobis earum, natus
                    iusto?
                </p>


            </div>
        </div>

    </div>
</template>