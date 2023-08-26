<script>

import { links } from './data/linkVideo.js';

import AppHeader from './components/AppHeader.vue';
import Jumbotron from './components/Jumbotron.vue';
import FeaturesHistory from './components/FeaturesHistory.vue';
import BannerCards from './components/BannerCards.vue';
import Concept from './components/Concept.vue';
import AppFooter from './components/AppFooter.vue';


export default {
  data() {
    return {
    };
  },
  components: { AppHeader, Jumbotron, BannerCards, Concept, FeaturesHistory, AppFooter },
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
  <BannerCards :links="linksData"></BannerCards>
  <Concept></Concept>
  <FeaturesHistory></FeaturesHistory>
  <AppFooter></AppFooter>
</template>

<style scoped></style>
