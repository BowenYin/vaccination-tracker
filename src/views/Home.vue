<template>
  <v-container>
    <v-row no-gutters>
      <v-col cols="12">
        <h2 class="text-center">How close to herd immunity?</h2>
      </v-col>
    </v-row>
    <v-row class="my-4">
      <v-spacer></v-spacer>
      <v-col cols="4">
        U.S. Vaccination Progress
        <v-row no-gutters>
          <v-col cols="auto">
            <svg xmlns="http://www.w3.org/2000/svg" width="360" height="25"  stroke="#000" stroke-linecap="round" stroke-linejoin="round" fill="#fff" fill-rule="evenodd" font-family="Roboto" font-size="14" text-anchor="middle"><g fill="#c1c1c1" stroke="#c1c1c1"><path stroke-linejoin="miter" d="M0 3h4v19H0z"/><path d="M5.5 12.5H47" stroke-linecap="square" stroke-width="4"/></g><g stroke="#b8d8c6"><path d="M312.5.5v23l20-11.5z" fill="#b8d8c6" stroke-linejoin="miter"/><path d="M332.5 12h27" fill="none" stroke-linecap="square" stroke-width="2"/></g><g stroke="none"><path fill="#b8d8c6" d="M49.5.5H312V24H49.5z"/><path fill="#f66" d="M49.5.5h10V24h-10z"/><path fill="#107c41" d="M224.5.5h50V24h-50z"/></g><g fill="none"><g stroke-linecap="butt"><path d="M49.5.5h265M49.5 24H312"/><path d="M49.5-.5v26"/></g><path d="M314.5.5l17.5 10h27.5M332 13h27.5m-47 11L332 13"/></g><text fill="#000" stroke="none"><tspan x="185" y="17.12">3.2%</tspan></text></svg>
          </v-col>
          <!-- <v-col cols="auto">
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
          </v-col> -->
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
