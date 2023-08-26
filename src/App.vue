<script>

import { links } from './data/linkVideo.js';

import AppHeader from './components/AppHeader.vue';
import Jumbotron from './components/Jumbotron.vue';
import FeaturesHistory from './components/FeaturesHistory.vue';
import BannerCards from './components/BannerCards.vue';
import Concept from './components/Concept.vue';


export default {
  data() {
    return {
    };
  },
  components: { AppHeader, Jumbotron, FeaturesHistory, BannerCards, Concept },
  computed: {
    linksData() {
      return links;
    }
  }
}


</script>

<template>
  <AppHeader></AppHeader>
  <Jumbotron></Jumbotron>
  <FeaturesHistory></FeaturesHistory>
  <BannerCards :links="linksData"></BannerCards>
  <Concept></Concept>
</template>

<style scoped></style>
