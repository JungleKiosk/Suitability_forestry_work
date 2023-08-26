<script>

import { links } from './data/linkVideo.js';

import AppHeader from './components/AppHeader.vue';
import Jumbotron from './components/Jumbotron.vue';
import FeaturesHistory from './components/FeaturesHistory.vue';
import BannerCards from './components/BannerCards.vue';
import Concept from './components/Concept.vue';
import AppFooter from './components/AppFooter.vue';
import FileCode from './components/FileCode.vue';



export default {
  data() {
    return {
    };
  },
  components: { AppHeader, BannerCards, Concept, Jumbotron, FeaturesHistory, AppFooter, FileCode },
  computed: {
    linksData() {
      return links;
    }
  }
}


</script>

<template>
  <AppHeader></AppHeader>
  <Concept></Concept>
  <FileCode></FileCode>
  <BannerCards :links="linksData"></BannerCards>
  <Jumbotron></Jumbotron>
  <FeaturesHistory></FeaturesHistory>
  <AppFooter></AppFooter>
</template>

<style scoped></style>
