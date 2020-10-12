<template>
<v-row>
    <v-col v-for="n in 3" :key="n" class="d-flex child-flex" cols="4">
    <v-card
        :loading="loading"
        class="mx-auto my-12"
        max-width="374"
    >
        <template slot="progress">
        <v-progress-linear
            color="deep-purple"
            height="10"
            indeterminate
        ></v-progress-linear>
        </template>

        <v-img
        height="250"
        src="../assets/irene2.jpg"
        ></v-img>

        <v-card-title>Basic Package</v-card-title>

        <v-card-text>
        <div class="my-4 subtitle-1">
            $ • "I don't have kids" Detail
        </div>

        <div><ul>
            <li>Premium hand wash, with a wash and wax solution to help protect and enrich the shine and protection on your Car/Truck</li>
            <li>Light vacuuming on seats and floors</li>
            <li>Dusting/ wipe down of dash and doors</li>
            <li>Windows cleaned inside and out</li>
    </ul>
    </div>
        </v-card-text>

        <v-divider class="mx-4"></v-divider>

        <v-card-title>Next Availability</v-card-title>

        <v-card-text>
        <v-chip-group
            v-model="selection"
            active-class="deep-purple accent-4 white--text"
            column
        >
            <v-chip>5:30PM</v-chip>

            <v-chip>7:30PM</v-chip>

            <v-chip>8:00PM</v-chip>

            <v-chip>9:00PM</v-chip>
        </v-chip-group>
        </v-card-text>

        <v-card-actions>
        <v-btn
            color="deep-purple lighten-2"
            text
            @click="reserve"
        >
            Reserve
        </v-btn>
        </v-card-actions>
    </v-card>
  </v-col>
</v-row>
</template>




<script>
import { Vue } from "vue-property-decorator";

  export default {
    name: 'SevicesCards',
    data: () => ({
      loading: false,
      selection: 1,
    }),

    methods: {
      reserve () {
        this.loading = true

        setTimeout(() => (this.loading = false), 2000)
      },
    },
  }
</script>