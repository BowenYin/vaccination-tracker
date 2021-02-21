<template>
  <v-app>
    <v-app-bar app color="accent" elevate-on-scroll>
      <a href="/" class="d-flex align-center text-decoration-none" style="color: inherit;">
        <h3 v-if="$vuetify.breakpoint.smAndUp">U.S. Vaccination Tracker</h3>
        <h4 v-else>U.S. Vaccination Tracker</h4>
      </a>

      <v-spacer></v-spacer>
      <!--<v-btn icon>
        <v-icon @click="$vuetify.theme.dark = !$vuetify.theme.dark">brightness_4</v-icon>
      </v-btn>-->
      <v-btn href="/about" text large :ripple="false">About</v-btn>
      <v-btn icon :ripple="false" @click="toggleDark">
        <v-icon>brightness_4</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <router-view></router-view>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',
  created() {
    this.$vuetify.theme.dark = localStorage.getItem("dark_mode") == "true";
  },
  components: {
  },

  data: () => ({
    //
  }),
  methods: {
    toggleDark() {
      localStorage.setItem("dark_mode", (!this.$vuetify.theme.dark).toString());
      location.reload();
    },
  }
};
</script>

<style>
  .flourish-credit {
    display: none !important;
  }
</style>