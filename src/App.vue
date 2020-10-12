<template>
  <v-app>
    <v-main>
      <home />
      <car-footer />
    </v-main>
  </v-app>
</template>

<script lang="ts">
import Vue from "vue";
import home from "./views/Home.vue";
import CarFooter from "./components/Footer.vue";

export default Vue.extend({
  name: "App",

  components: {
    home,
    CarFooter
  },

  data: () => ({
    //
  })
});
</script>
