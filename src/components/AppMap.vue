
<script>
import { LMap, LTileLayer, LMarker, LTooltip, LPopup } from "@vue-leaflet/vue-leaflet";


export default {
    props: {
        marker_points: {
            type: Array,
            required: true
        }
    },
    components: {
        LMap,
        LTileLayer,
        LMarker,
        LTooltip,
        LPopup
    },
    data() {
        return {
            url_osm: 'https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png',
            attribution:
                '&copy; <a target="_blank" href="http://osm.org/copyright">OpenStreetMap</a> contributors',
            zoom: 10,
            center: [43.976909, 11.777171],
            selectedMarker: null
        };
    },
    methods: {
        getImagePath: function (name) {
            return new URL(`../assets/img/${name}`, import.meta.url).href
        },
        selectMarker: function (marker) {
            this.selectedMarker = marker;
        },
        selectImage(image) {
            this.selectedMarker.img_popup = image.img_card;
        },
        closeMarkerCard() {
            this.selectedMarker = null;
        }
    }
}


</script>
  
  
<template>
    <div id="app_map" class="container my-3">
        <div class="row justify-content-center">
            <div class="col-12 col-lg-6">

                <l-map style="height: 500px;" :zoom="zoom" :center="center">
                    <l-tile-layer :url="url_osm" :attribution="attribution"></l-tile-layer>

                    <template v-for="(coordinate, index) in marker_points" :key="index">
                        <l-marker :lat-lng="[coordinate.lat, coordinate.long]" @click="selectMarker(coordinate)">
                            <l-tooltip>
                                <div>
                                    <!-- <p>id: {{ coordinate.id }}</p> -->
                                    <p>{{ coordinate.place }}</p>
                                    <p>{{ coordinate.lat }} , {{ coordinate.long }}</p>
                                </div>
                            </l-tooltip>
                            <l-popup class="popup">
                                <div>
                                    <!-- <p>id: {{ coordinate.id }}</p> -->
                                    <div class="row align-items-center row_images">
                                        <div class="col-6 my-2 img_slider"
                                            v-for="(image, imageIndex) in coordinate.img_marker_card" :key="imageIndex">
                                            <img :src="getImagePath(image.img_card)" :alt="image.img_card" class="img-fluid"
                                                @click="selectImage(image)" />
                                        </div>
                                    </div>
                                    <img class="p-2 rounded-5" :src="getImagePath(selectedMarker?.img_popup)" alt="img" />
                                    <p>{{ coordinate.place }}</p>
                                    <p>Coordinates: {{ coordinate.lat }} , {{ coordinate.long }}</p>
                                </div>
                            </l-popup>
                        </l-marker>
                    </template>
                </l-map>
            </div>



        </div>
        <!-- /.row -->
    </div>
    <!-- /.container -->
</template>