<template>
  <v-container>
    <v-row class="my-4">
      <v-spacer></v-spacer>
      <v-col cols="4">
        U.S. Vaccination Progress
        <v-row no-gutters>
          <v-col cols="auto">
            <svg xmlns="http://www.w3.org/2000/svg" width="48" height="24"  stroke="#c1c1c1" stroke-linecap="round" stroke-linejoin="round" fill="#c1c1c1" fill-rule="evenodd"><path stroke-linejoin="miter" d="M0 2h4v19H0z"/><path d="M5.5 11.5H47" stroke-linecap="square" stroke-width="4"/></svg>
          </v-col>
          <v-col>
            <v-progress-linear value="3.2" height="24">3.2%</v-progress-linear>
          </v-col>
          <v-col cols="auto">
            <svg xmlns="http://www.w3.org/2000/svg" width="48" height="24" stroke="#b8d8c6" stroke-linecap="round"
              stroke-linejoin="round" fill="#fff" fill-rule="evenodd">
              <path fill="#b8d8c6" d="M0 0v23l20-11.5z" stroke-linejoin="miter" />
              <path fill="none" d="M20 11.5h27" stroke-linecap="square" stroke-width="2" /></svg>
          </v-col>
        </v-row>
      </v-col>
      <v-spacer></v-spacer>
    </v-row>
    <div class="flourish-embed flourish-map" data-src="visualisation/4988587"></div>
    <v-row class="text-center">
  
      <v-col cols="12">
      </v-col>
    </v-row>
    <div class="flourish-embed flourish-table" data-src="visualisation/4989564"></div>
    <v-row>
      <p class="caption">Herd immunity occurs when enough people have protection from COVID-19 that the rest of the population is indirectly protected. There is no consensus on the exact percentage, but many experts now suggest that 70-85% is accurate. Learn more <a href="/about">here</a>.</p>
    </v-row>
  </v-container>
</template>

<script>

export default {
  name: 'Home',
  components: {
  }
}
</script>
