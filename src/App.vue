<template>
  <v-app>
    <v-app-bar app color="white" elevate-on-scroll>
      <div class="d-flex align-center">
        <h3>Vaccination Tracker</h3>
      </div>

      <v-spacer></v-spacer>

      
    </v-app-bar>

    <v-main>
    
      <v-container>
        <v-row class="my-4">
          <v-spacer></v-spacer>
          <v-col cols="4">
          U.S. Vaccination Progress
          <v-progress-linear value="1" height="16"></v-progress-linear>1%
          </v-col>
          <v-spacer></v-spacer>
        </v-row>
        <div class="flourish-embed flourish-map" data-src="visualisation/4988587"></div>
        <v-row class="text-center">
          
          <v-col cols="12">
          </v-col>
        </v-row>
        <div class="flourish-embed flourish-table" data-src="visualisation/4989564"></div>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  components: {
  },

  data: () => ({
    //
  }),
};
</script>

<style>
  .flourish-credit {
    display: none !important;
  }
</style>