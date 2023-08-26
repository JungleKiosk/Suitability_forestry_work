<script>

export default {
    props: ['links'],
    data() {
        return {

        };
    },
    methods: {
        getImagePath: function (name) {
            return new URL(`../assets/img/${name}`, import.meta.url).href
        }
    }
}

</script>

<template>

    <div class="container my-2">
        <div class="row align-items-stretch justify-content-center">

            <div v-for="link in links" :key="link.title" class="col-12 col-lg-4 col-md-6">
                <div class="card rounded-4 bg_card my-3 d-flex bg_item">
                    <div class="card-header title" style="font-size: large;">
                        {{ link.title }}
                    </div>

                    <div class="card-body d-flex flex-column">
                        <p>{{ link.desc }}</p>
                        <img class="rounded-4 card_img_zoom" :src="getImagePath(link.img)" alt="Image"
                            style="height: 200px;" />
                        <div class="link_video py-1 text-center">
                            <a class="title" :href="link.video" target="_blank">
                                Go to video
                                <img class="yt_icon" src="./../assets/img/icons/yt.svg" alt="">
                            </a>
                        </div>
                    </div>

                </div>
            </div>
        </div>
    </div>
</template>
  

<style>
img {
    width: 100%;
}

.link_video a {
    text-decoration: none;
}

.yt_icon {
    width: 20%;
}

.yt_icon {
    transition: transform 0.2s ease-in-out;
    transform-origin: center center;
}

.yt_icon:hover {
    transform: scale(1.3);
}
</style>