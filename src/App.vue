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
import Vuetify from "/Users/paigewalters/Desktop/VueApps/precision-polish/node_modules/vuetify";
import home from "./views/Home.vue";
import CarFooter from "./components/Footer.vue";

Vue.use(Vuetify)

export default Vue.extend({
  name: "App",

  components: {
    home,
    CarFooter,
  },

  data: () => ({
    //
  })
});
</script>
