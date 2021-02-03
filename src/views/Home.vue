<template>
  <v-container>
    <v-row no-gutters>
      <v-col cols="12">
        <h1 class="text-center">How close to herd immunity?</h1>
      </v-col>
    </v-row>
    <v-row class="mt-1">
      <v-col cols="12">
        <v-row no-gutters>
          <v-spacer></v-spacer>
          <v-col cols="auto">
            <!-- <svg xmlns="http://www.w3.org/2000/svg" width="360" height="25"  stroke="#000" stroke-linecap="round" stroke-linejoin="round" fill="#fff" fill-rule="evenodd" font-family="Roboto" font-size="14" text-anchor="middle"><g fill="#c1c1c1" stroke="#c1c1c1"><path stroke-linejoin="miter" d="M0 3h4v19H0z"/><path d="M5.5 12.5H47" stroke-linecap="square" stroke-width="4"/></g><g stroke="#b8d8c6"><path d="M312.5.5v23l20-11.5z" fill="#b8d8c6" stroke-linejoin="miter"/><path d="M332.5 12h27" fill="none" stroke-linecap="square" stroke-width="2"/></g><g stroke="none"><path fill="#b8d8c6" d="M49.5.5H312V24H49.5z"/><path fill="#f66" d="M49.5.5h10V24h-10z"/><path fill="#107c41" d="M224.5.5h50V24h-50z"/></g><g fill="none"><g stroke-linecap="butt"><path d="M49.5.5h265M49.5 24H312"/><path d="M49.5-.5v26"/></g><path d="M314.5.5l17.5 10h27.5M332 13h27.5m-47 11L332 13"/></g><text fill="#000" stroke="none"><tspan x="185" y="17.12">3.2%</tspan></text></svg> -->
            <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:v="http://vecta.io" width="480" height="100" viewBox="0 0 480 100"><defs><pattern id="kkam3c1fcmz" patternUnits="userSpaceOnUse" width="4" height="6" patternTransform="rotate(-45 2 2)"><path d="M -1,2 l 6,0" stroke="#0078D4" stroke-opacity="0.8" stroke-width="2"/></pattern></defs><rect fill="#000000" height="36" stroke-width="0" width="6" x="0" y="0" transform="translate(-0.5 31.5)"/><rect fill="#000000" height="6" stroke-width="0" width="50" x="0" y="0" transform="translate(5.5 46.5)"/><rect fill="#000000" height="40" stroke-width="0" width="3" x="0" y="0" transform="translate(55.5 29.5)"/><rect fill="#000000" height="3" stroke-width="0" width="331" x="0" y="0" transform="translate(58.5 29.5)"/><rect fill="#000000" height="3" stroke-width="0" width="331" x="0" y="0" transform="translate(58.5 66.5)"/><rect fill="#000000" height="3" stroke-width="0" width="30.5087" x="0" y="0" transform="translate(384.9438 38.9292) rotate(40 15.2544 1.5)"/><rect fill="#000000" height="3" stroke-width="0" width="30.3855" x="0" y="0" transform="translate(384.9582 57.1104) rotate(320 15.1927 1.5)"/><rect x="0" y="0" width="71" height="2" stroke-width="0" fill="#000000" transform="translate(408.5 47)"/><rect x="0" y="0" width="71" height="2" stroke-width="0" fill="#000000" transform="translate(408.5 50)"/><rect x="0" y="0" width="6" height="1" stroke-width="0" fill="#fffffe" transform="translate(407.5 49)"/><rect x="58.5" y="32.5" :width="vaccinatedWidth" height="34" stroke-width="0" fill="#21A366"/><g transform="translate(304.5 32.5)"><svg x="0" y="0" width="52" height="34" class="Ignore.cls" stroke="initial" stroke-linecap="initial" stroke-linejoin="initial" fill="initial" text-anchor="initial" fill-rule="initial" viewBox="0 0 52 34"><rect x="0" y="0" width="100%" height="100%" fill="url(#kkam3c1fcmz)"/></svg><rect x="0" y="0" width="52" height="34" class="Rim.cls" stroke="none" fill="none"/></g><rect x="0" y="0" width="2" height="34" stroke-width="0" fill="#0078D4" fill-opacity="0.8" transform="translate(302.5 32.5)"/><rect x="0" y="0" width="2" height="34" stroke-width="0" fill="#0078D4" fill-opacity="0.8" transform="translate(356.5 32.5)"/><g transform="translate(301.5 2.5)"><rect x="0" y="0" width="51" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="51" height="13" fill="none" stroke="none"/><text fill="#000000" fill-opacity="1" font-family="Source Sans Pro" font-weight="bold" text-anchor="start"><tspan x="2" y="11.12">70-85%</tspan></text></g></g><g transform="translate(301.5 15.5)"><rect x="0" y="0" width="72" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="72" height="13" fill="none" stroke="none"/><text fill="#000000" fill-opacity="1" font-family="Source Sans Pro" font-size="11px" text-anchor="start"><tspan x="2" y="10.13">herd immunity</tspan></text></g></g><rect :x="vaccinatedWidth+58" y="32.5" :width="recoveredWidth" height="34" stroke-width="0" fill="#838383"/><g :transform="`translate(${vaccinatedWidth+16} 2.5)`"><rect x="0" y="0" width="45" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="45" height="13" fill="none" stroke="none"/><text fill="#000000" fill-opacity="1" font-family="Source Sans Pro" font-weight="bold" text-anchor="end"><tspan x="43" y="11.12">{{vaccinatedPct}}%</tspan></text></g></g><g :transform="`translate(${vaccinatedWidth+7} 15.5)`"><rect x="0" y="0" width="54" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="54" height="13" fill="none" stroke="none"/><text fill="#000000" fill-opacity="1" font-family="Source Sans Pro" font-size="11px" text-anchor="end"><tspan x="52" y="10.13">vaccinated</tspan></text></g></g><g :transform="`translate(${vaccinatedWidth+recoveredWidth+56} 2.5)`"><rect x="0" y="0" width="45" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="45" height="13" fill="none" stroke="none"/><text fill="#000000" fill-opacity="1" font-family="Source Sans Pro" font-weight="bold" text-anchor="start"><tspan x="2" y="11.12">{{recoveredPct}}%</tspan></text></g></g><g :transform="`translate(${vaccinatedWidth+recoveredWidth+56} 15.5)`"><rect x="0" y="0" width="50" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="50" height="13" fill="none" stroke="none"/><text fill="#000000" fill-opacity="1" font-family="Source Sans Pro" font-size="11px" text-anchor="start"><tspan x="2" y="10.13">recovered</tspan></text></g></g><g :transform="`translate(${vaccinatedWidth+16} 70.5)`"><rect x="0" y="0" width="45" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="45" height="13" fill="none" stroke="none"/><text fill="#000000" fill-opacity="1" font-family="Source Sans Pro" font-weight="bold" text-anchor="end" font-size="12px"><tspan x="43" y="10.46">+{{pastWkChange}}%</tspan></text></g></g><g :transform="`translate(${vaccinatedWidth} 81.5)`"><rect x="0" y="0" width="61" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="61" height="13" fill="none" stroke="none"/><text fill="#000000" fill-opacity="1" font-family="Source Sans Pro" font-size="10px" text-anchor="end"><tspan x="59" y="9.8">in past week</tspan></text></g></g></svg>
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
          <v-spacer></v-spacer>
        </v-row>
      </v-col>
    </v-row>
    <div class="flourish-embed flourish-map" data-src="visualisation/4988587"></div>
    <v-row class="text-center">
  
      <v-col cols="12">
      </v-col>
    </v-row>
    <div class="flourish-embed flourish-table" data-src="visualisation/4989564"></div>
    <v-row>
      <v-col>
        <p class="body-2">Herd immunity occurs when enough people have protection from COVID-19 that the rest of the population is indirectly protected. Reaching herd immunity will result in declining infections but will not stop the pandemic entirely. There is no consensus on the exact percentage, but many experts now suggest that 70-85% is an accurate benchmark for herd immunity. Read more about our data and methods <a href="/about">here</a>.</p>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>

export default {
  name: 'Home',
  components: {
  },
  data: () => ({
    vaccinatedWidth: 350*0.077,
    recoveredWidth: 350*0.030,
    vaccinatedPct: 7.7,
    recoveredPct: 3.0,
    pastWkChange: 2.9,
  }),
}
</script>
