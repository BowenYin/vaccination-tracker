<template>
  <div class="home">
    <v-container>
      <v-row class="text-center">
        <v-col cols="12">
          <iframe src='https://flo.uri.sh/visualisation/4913802/embed' title='Interactive or visual content' frameborder='0' scrolling='no' style='width:100%;height:600px;'></iframe><div style='width:100%!;margin-top:4px!important;text-align:right!important;'><a class='flourish-credit' href='https://public.flourish.studio/visualisation/4913802/?utm_source=embed&utm_campaign=visualisation/4913802' target='_top' style='text-decoration:none!important'><img alt='Made with Flourish' src='https://public.flourish.studio/resources/made_with_flourish.svg' style='width:105px!important;height:16px!important;border:none!important;margin:0!important;'> </a></div>
        </v-col>

        <v-col class="mb-4">
          

          <p class="subheading font-weight-regular">
            For help and collaboration with other Vuetify developers,
            <br>please join our online
            <a
              href="https://community.vuetifyjs.com"
              target="_blank"
            >Discord Community</a>
          </p>
        </v-col>

        <v-col
          class="mb-5"
          cols="12"
        >
          <h2 class="headline font-weight-bold mb-3">
            What's next?
          </h2>

          <v-row justify="center">
            <a
              v-for="(next, i) in whatsNext"
              :key="i"
              :href="next.href"
              class="subheading mx-3"
              target="_blank"
            >
              {{ next.text }}
            </a>
          </v-row>
        </v-col>

      </v-row>
    </v-container>
  </div>
</template>

<script>

export default {
  name: 'Home',
  components: {
  }
}
</script>
