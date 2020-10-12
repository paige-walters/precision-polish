<template>
  <container class="home">
    <div><home-header /></div>
    <div><services-cards /></div>
    <div><car-carousel /></div>
  </container>
</template>


<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";
import HomeHeader from "../components/HomeHeader.vue";
import CarCarousel from "../components/CarCarousel.vue";
import ServicesCards from '../components/ServicesCards.vue';

export default Vue.extend({
    components: {
    HomeHeader,
    CarCarousel,
    ServicesCards
  }
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>