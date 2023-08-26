<script>

import AppHeader from './components/AppHeader.vue';
import Jumbotron from './components/Jumbotron.vue';
import FeaturesHistory from './components/FeaturesHistory.vue';


export default {
  data() {
    return {
    };
  },
  components: { AppHeader, Jumbotron, FeaturesHistory }
}


</script>

<template>
  <AppHeader></AppHeader>
  <Jumbotron></Jumbotron>
  <FeaturesHistory></FeaturesHistory>
</template>

<style scoped>


</style>
