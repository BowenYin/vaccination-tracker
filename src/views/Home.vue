<template>
  <v-container>
    <v-row no-gutters>
      <v-col cols="12">
        <h1 v-if="$vuetify.breakpoint.smAndUp" class="text-center">How close to herd immunity?<span class="font-weight-regular">*</span></h1>
        <h2 v-else class="text-center">How close to herd immunity?<span class="font-weight-regular">*</span></h2>
        <h4 class="text-center">This site is no longer regularly updated. Last update: 5/29/21</h4>
      </v-col>
    </v-row>
    <v-row class="mt-1">
      <v-col cols="12">
        <v-row no-gutters>
          <v-spacer></v-spacer>
          <v-col cols="auto">
            <!-- <svg xmlns="http://www.w3.org/2000/svg" width="360" height="25"  stroke="#000" stroke-linecap="round" stroke-linejoin="round" fill="#fff" fill-rule="evenodd" font-family="Roboto" font-size="14" text-anchor="middle"><g fill="#c1c1c1" stroke="#c1c1c1"><path stroke-linejoin="miter" d="M0 3h4v19H0z"/><path d="M5.5 12.5H47" stroke-linecap="square" stroke-width="4"/></g><g stroke="#b8d8c6"><path d="M312.5.5v23l20-11.5z" fill="#b8d8c6" stroke-linejoin="miter"/><path d="M332.5 12h27" fill="none" stroke-linecap="square" stroke-width="2"/></g><g stroke="none"><path fill="#b8d8c6" d="M49.5.5H312V24H49.5z"/><path fill="#f66" d="M49.5.5h10V24h-10z"/><path fill="#107c41" d="M224.5.5h50V24h-50z"/></g><g fill="none"><g stroke-linecap="butt"><path d="M49.5.5h265M49.5 24H312"/><path d="M49.5-.5v26"/></g><path d="M314.5.5l17.5 10h27.5M332 13h27.5m-47 11L332 13"/></g><text fill="#000" stroke="none"><tspan x="185" y="17.12">3.2%</tspan></text></svg> -->
            <svg v-if="$vuetify.theme.dark" class="syringe" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:v="http://vecta.io" width="480" height="100" viewBox="0 0 480 100"><defs><pattern id="kkam3c1fcmz" patternUnits="userSpaceOnUse" width="4" height="6" patternTransform="rotate(-45 2 2)"><path d="M -1,2 l 6,0" stroke="#0078D4" stroke-opacity="0.8" stroke-width="2"/></pattern></defs><rect fill="#FFFFFF" height="36" stroke-width="0" width="6" x="0" y="0" transform="translate(-0.5 31.5)"/><rect fill="#FFFFFF" height="6" stroke-width="0" width="50" x="0" y="0" transform="translate(5.5 46.5)"/><rect fill="#FFFFFF" height="40" stroke-width="0" width="3" x="0" y="0" rx="1.5" transform="translate(55.5 29.5)"/><rect fill="#FFFFFF" height="3" stroke-width="0" width="335" x="0" y="0" rx="1.5" transform="translate(55.5 29.5)"/><rect fill="#FFFFFF" height="3" stroke-width="0" width="335" x="0" y="0" rx="1.5" transform="translate(55.5 66.5)"/><rect fill="#FFFFFF" height="3" stroke-width="0" width="30.5087" x="0" y="0" rx="1.5" transform="translate(384.9438 38.9292) rotate(40 15.2544 1.5)"/><rect fill="#FFFFFF" height="3" stroke-width="0" width="30.3855" x="0" y="0" rx="1.5" transform="translate(384.9582 57.1104) rotate(320 15.1927 1.5)"/><rect fill="#FFFFFF" height="2" stroke-width="0" width="70" x="0" y="0" transform="translate(409.5 48.5)"/><rect x="58.5" y="32.5" :width="fullVaxWidth" height="34" stroke-width="0" fill="#21A366"/><g transform="translate(304.5 32.5)"><svg x="0" y="0" width="52" height="34" class="Ignore.cls" stroke="initial" stroke-linecap="initial" stroke-linejoin="initial" fill="initial" text-anchor="initial" fill-rule="initial" viewBox="0 0 52 34"><rect x="0" y="0" width="100%" height="100%" fill="url(#kkam3c1fcmz)"/></svg><rect x="0" y="0" width="52" height="34" class="Rim.cls" stroke="none" fill="none"/></g><rect fill="#0078D4" fill-opacity="0.8" height="34" stroke-width="0" width="2" x="0" y="0" transform="translate(302.5 32.5)"/><rect fill="#0078D4" fill-opacity="0.8" height="34" stroke-width="0" width="2" x="0" y="0" transform="translate(356.5 32.5)"/><g transform="translate(301.5 2.5)"><rect fill="none" height="13" stroke="none" stroke-width="0" width="51" x="0" y="0"/><g><rect x="0" y="0" width="51" height="13" fill="none" stroke="none"/><text fill="#FFFFFF" fill-opacity="1" font-family="Source Sans Pro" font-weight="bold" text-anchor="start"><tspan x="2" y="11.12">70-85%</tspan></text></g></g><g transform="translate(301.5 15.5)"><rect x="0" y="0" width="72" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="72" height="13" fill="none" stroke="none"/><text fill="#FFFFFF" fill-opacity="1" font-family="Source Sans Pro" font-size="11px" text-anchor="start"><tspan x="2" y="10.13">herd immunity</tspan></text></g></g><rect :x="fullVaxWidth+58" y="32.5" :width="vaxWidth" height="34" stroke-width="0" fill="#33C481"/><g :transform="`translate(${fullVaxWidth+16} 2.5)`"><rect x="0" y="0" width="45" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="45" height="13" fill="none" stroke="none"/><text fill="#FFFFFF" fill-opacity="1" font-family="Source Sans Pro" font-weight="bold" text-anchor="end"><tspan x="43" y="11.12">{{fullVaccinatedPct}}%</tspan></text></g></g><g :transform="`translate(${fullVaxWidth+7} 15.5)`"><rect x="0" y="0" width="54" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="54" height="13" fill="none" stroke="none"/><text fill="#FFFFFF" fill-opacity="1" font-family="Source Sans Pro" font-size="11px" text-anchor="end"><tspan x="52" y="10.13">vaccinated</tspan></text></g></g><g :transform="`translate(${fullVaxWidth+vaxWidth+56} 2.5)`"><rect x="0" y="0" width="45" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="45" height="13" fill="none" stroke="none"/><text fill="#FFFFFF" fill-opacity="1" font-family="Source Sans Pro" font-weight="bold" text-anchor="start"><tspan x="2" y="11.12">{{vaccinatedPct}}%</tspan></text></g></g><g :transform="`translate(${fullVaxWidth+vaxWidth+56} 15.5)`"><rect x="0" y="0" width="50" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="50" height="13" fill="none" stroke="none"/><text fill="#FFFFFF" fill-opacity="1" font-family="Source Sans Pro" font-size="11px" text-anchor="start"><tspan x="2" y="10.13">partially</tspan></text></g></g><g :transform="`translate(${fullVaxWidth+vaxWidth+16} 70.5)`"><rect x="0" y="0" width="45" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="45" height="13" fill="none" stroke="none"/><text fill="#FFFFFF" fill-opacity="1" font-family="Source Sans Pro" font-weight="bold" text-anchor="start" font-size="12px"><tspan x="42" y="10.46">+{{pastWkChange}}%</tspan></text></g></g><g :transform="`translate(${fullVaxWidth+vaxWidth} 81.5)`"><rect x="0" y="0" width="61" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="61" height="13" fill="none" stroke="none"/><text fill="#FFFFFF" fill-opacity="1" font-family="Source Sans Pro" font-size="10px" text-anchor="start"><tspan x="58" y="9.8">in past week</tspan></text></g></g></svg>
            <svg v-else class="syringe" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:v="http://vecta.io" width="480" height="100" viewBox="0 0 480 100"><defs><pattern id="kkam3c1fcmz" patternUnits="userSpaceOnUse" width="4" height="6" patternTransform="rotate(-45 2 2)"><path d="M -1,2 l 6,0" stroke="#0078D4" stroke-opacity="0.8" stroke-width="2"/></pattern></defs><rect fill="#000000" height="36" stroke-width="0" width="6" x="0" y="0" transform="translate(-0.5 31.5)"/><rect fill="#000000" height="6" stroke-width="0" width="50" x="0" y="0" transform="translate(5.5 46.5)"/><rect fill="#000000" height="40" stroke-width="0" width="3" x="0" y="0" rx="1.5" transform="translate(55.5 29.5)"/><rect fill="#000000" height="3" stroke-width="0" width="335" x="0" y="0" rx="1.5" transform="translate(55.5 29.5)"/><rect fill="#000000" height="3" stroke-width="0" width="335" x="0" y="0" rx="1.5" transform="translate(55.5 66.5)"/><rect fill="#000000" height="3" stroke-width="0" width="30.5087" x="0" y="0" rx="1.5" transform="translate(384.9438 38.9292) rotate(40 15.2544 1.5)"/><rect fill="#000000" height="3" stroke-width="0" width="30.3855" x="0" y="0" rx="1.5" transform="translate(384.9582 57.1104) rotate(320 15.1927 1.5)"/><rect fill="#000000" height="2" stroke-width="0" width="70" x="0" y="0" transform="translate(409.5 48.5)"/><rect x="58.5" y="32.5" :width="fullVaxWidth" height="34" stroke-width="0" fill="#21A366"/><g transform="translate(304.5 32.5)"><svg x="0" y="0" width="52" height="34" class="Ignore.cls" stroke="initial" stroke-linecap="initial" stroke-linejoin="initial" fill="initial" text-anchor="initial" fill-rule="initial" viewBox="0 0 52 34"><rect x="0" y="0" width="100%" height="100%" fill="url(#kkam3c1fcmz)"/></svg><rect x="0" y="0" width="52" height="34" class="Rim.cls" stroke="none" fill="none"/></g><rect fill="#0078D4" fill-opacity="0.8" height="34" stroke-width="0" width="2" x="0" y="0" transform="translate(302.5 32.5)"/><rect fill="#0078D4" fill-opacity="0.8" height="34" stroke-width="0" width="2" x="0" y="0" transform="translate(356.5 32.5)"/><g transform="translate(301.5 2.5)"><rect fill="none" height="13" stroke="none" stroke-width="0" width="51" x="0" y="0"/><g><rect x="0" y="0" width="51" height="13" fill="none" stroke="none"/><text fill="#000000" fill-opacity="1" font-family="Source Sans Pro" font-weight="bold" text-anchor="start"><tspan x="2" y="11.12">70-85%</tspan></text></g></g><g transform="translate(301.5 15.5)"><rect x="0" y="0" width="72" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="72" height="13" fill="none" stroke="none"/><text fill="#000000" fill-opacity="1" font-family="Source Sans Pro" font-size="11px" text-anchor="start"><tspan x="2" y="10.13">herd immunity</tspan></text></g></g><rect :x="fullVaxWidth+58" y="32.5" :width="vaxWidth" height="34" stroke-width="0" fill="#33C481"/><g :transform="`translate(${fullVaxWidth+16} 2.5)`"><rect x="0" y="0" width="45" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="45" height="13" fill="none" stroke="none"/><text fill="#000000" fill-opacity="1" font-family="Source Sans Pro" font-weight="bold" text-anchor="end"><tspan x="43" y="11.12">{{fullVaccinatedPct}}%</tspan></text></g></g><g :transform="`translate(${fullVaxWidth+7} 15.5)`"><rect x="0" y="0" width="54" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="54" height="13" fill="none" stroke="none"/><text fill="#000000" fill-opacity="1" font-family="Source Sans Pro" font-size="11px" text-anchor="end"><tspan x="52" y="10.13">vaccinated</tspan></text></g></g><g :transform="`translate(${fullVaxWidth+vaxWidth+56} 2.5)`"><rect x="0" y="0" width="45" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="45" height="13" fill="none" stroke="none"/><text fill="#000000" fill-opacity="1" font-family="Source Sans Pro" font-weight="bold" text-anchor="start"><tspan x="2" y="11.12">{{vaccinatedPct}}%</tspan></text></g></g><g :transform="`translate(${fullVaxWidth+vaxWidth+56} 15.5)`"><rect x="0" y="0" width="50" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="50" height="13" fill="none" stroke="none"/><text fill="#000000" fill-opacity="1" font-family="Source Sans Pro" font-size="11px" text-anchor="start"><tspan x="2" y="10.13">partially</tspan></text></g></g><g :transform="`translate(${fullVaxWidth+vaxWidth+16} 70.5)`"><rect x="0" y="0" width="45" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="45" height="13" fill="none" stroke="none"/><text fill="#000000" fill-opacity="1" font-family="Source Sans Pro" font-weight="bold" text-anchor="start" font-size="12px"><tspan x="42" y="10.46">+{{pastWkChange}}%</tspan></text></g></g><g :transform="`translate(${fullVaxWidth+vaxWidth} 81.5)`"><rect x="0" y="0" width="61" height="13" fill="none" stroke="none" stroke-width="0"/><g><rect x="0" y="0" width="61" height="13" fill="none" stroke="none"/><text fill="#000000" fill-opacity="1" font-family="Source Sans Pro" font-size="10px" text-anchor="start"><tspan x="58" y="9.8">in past week</tspan></text></g></g></svg>
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
    <div v-if="$vuetify.theme.dark" class="flourish-embed flourish-map" data-src="visualisation/5351876"></div>
    <div v-else class="flourish-embed flourish-map" data-src="visualisation/4988587"></div>
    <div v-if="$vuetify.theme.dark" class="flourish-embed flourish-table" data-src="visualisation/5352482"></div>
    <div v-else class="flourish-embed flourish-table" data-src="visualisation/4989564"></div>
    <v-row justify="space-around">
      <v-col cols="auto">
        <p class="body-2" style="max-width: 1000px;">*Herd immunity occurs when enough people have protection from COVID-19 that the rest of the population is indirectly protected. Reaching herd immunity will result in declining infections but will not stop the pandemic entirely. There is no consensus on the exact percentage, but many experts now suggest that 70-85% is an accurate benchmark for herd immunity. Read more about our data and methods <a href="/about">here</a>.</p>
      </v-col>
    </v-row>
    <v-row justify="center" align="center" class="mt-0 mb-4">
      <v-col cols="auto">
        <div class="body-1">Follow us to stay updated!</div>
      </v-col>
      <v-col cols="auto" style="height: 48px;">
        <a href="https://twitter.com/vaccinprogress" target="_blank">
          <img src="../assets/twitter.svg" height="24">
        </a>
      </v-col>
      <v-col cols="auto" style="height: 48px;">
        <a href="https://www.facebook.com/vaccineprogressinfo" target="_blank">
          <img src="../assets/facebook.svg" height="24">
        </a>
      </v-col>
      <v-col cols="auto" style="height: 48px;">
        <a href="https://www.linkedin.com/company/vaccine-progress-info/" target="_blank">
          <img src="../assets/linkedin.svg" height="24">
        </a>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
const vaxPct = window.vaxData?.vax || 15.9;
const fullVaxPct = window.vaxData?.fullVax || 8.1;
export default {
  name: 'Home',
  components: {
  },
  data: () => ({
    fullVaxWidth: 350*parseFloat((fullVaxPct/100.0).toFixed(3)),
    vaxWidth: 350*parseFloat(((vaxPct-fullVaxPct)/100.0).toFixed(3)),
    fullVaccinatedPct: fullVaxPct,
    vaccinatedPct: vaxPct,
    pastWkChange: window.vaxData?.wk || 2.3,
  }),
}
</script>

<style scoped>
.syringe {
  max-width: 100%;
}
</style>