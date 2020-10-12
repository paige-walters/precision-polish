<template>
  <container class="home">
    <div><home-header /></div>
    <div><car-carousel /></div>
  </container>
</template>


<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";
import HomeHeader from "../components/HomeHeader.vue";
import CarCarousel from "../components/CarCarousel.vue";

export default Vue.extend({
    components: {
    HomeHeader,
    CarCarousel
  }
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>