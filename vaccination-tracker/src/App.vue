<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
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
        Vaccination Progress
        <v-progress-linear value="1"></v-progress-linear>
        </v-col>
        <v-spacer></v-spacer>
      </v-row>
      <v-row class="text-center">
        
        <v-col cols="12">
        <iframe src='https://flo.uri.sh/visualisation/4913802/embed' title='Interactive or visual content' frameborder='0' scrolling='no' style='width:100%;height:600px;'></iframe><div style='width:100%!;margin-top:4px!important;text-align:right!important;'><a class='flourish-credit' href='https://public.flourish.studio/visualisation/4913802/?utm_source=embed&utm_campaign=visualisation/4913802' target='_top' style='text-decoration:none!important'><img alt='Made with Flourish' src='https://public.flourish.studio/resources/made_with_flourish.svg' style='width:105px!important;height:16px!important;border:none!important;margin:0!important;'> </a></div>
        </v-col>
        </v-row>
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
