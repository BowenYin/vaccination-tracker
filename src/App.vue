<template>
  <v-app>
    <v-app-bar app color="white" elevate-on-scroll>
      <div class="d-flex align-center">
        <h3>Vaccination Tracker</h3>
      </div>

      <v-spacer></v-spacer>

      
    </v-app-bar>

    <v-main>
      <router-view></router-view>
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