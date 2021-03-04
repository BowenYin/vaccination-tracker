<template>
  <v-container>
    <v-row>
      <v-col cols="12">
        <v-alert dense outlined>Herd immunity occurs when enough people have protection from COVID-19 that the rest of the population is indirectly protected. Reaching herd immunity will result in declining infections but will not stop the pandemic entirely. There is no consensus on the exact percentage, but many experts now suggest that 70-85% is an accurate benchmark for herd immunity. See more about herd immunity and data below.</v-alert>
        <h2>Data in Detail</h2>
        <h3>Herd Immunity</h3>
        <p>There are <a href="https://www.jhsph.edu/covid-19/articles/achieving-herd-immunity-with-covid19.html" target="_blank">two paths</a> to immunity: 1) exposure and infection with the virus and 2) vaccination. Encountering the virus is <a href="https://www.nature.com/articles/d41586-020-02948-4" target="_blank">extremely unsafe</a> without a vaccine, but both ways result in the body producing antibodies against COVID-19. During herd immunity conditions, the average number of other people an infected person will infect should be <a href="https://www.nature.com/articles/d41586-020-02009-w" target="_blank">roughly below 1</a>. This means the disease is declining. See data sourcing below on why we only present vaccinated data in our tracker.</p>
        <p>Dr. Anthony Fauci, director of the National Institute of Allergy and Infectious Diseases, said in an <a href="https://www.nytimes.com/2020/12/24/health/herd-immunity-covid-coronavirus.html" target="_blank">interview</a> that 70-85% is a fair estimate for true herd immunity. Researchers have used <a href="https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7236739/" target="_blank">quantitative models</a> to find herd immunity levels in a similar ballpark.</p>
        <p>However, it is worth noting that new strains of the virus have emerged which are <a href="https://www.cdc.gov/coronavirus/2019-ncov/more/science-and-research/scientific-brief-emerging-variants.html" target="_blank">more contagious</a> than the initial strain. These strains will raise the herd immunity threshold. These thresholds also heavily rely on population density, adherence to public health measures (such as washing hands, mask-wearing), and the strain of the virus.</p>
        <h3>Data Sourcing</h3>
        <p>Vaccination data comes from the <a href="https://covid.cdc.gov/covid-data-tracker/#vaccinations" target="_blank">CDC</a>. Data on COVID-19 recoveries comes from <a href="https://www.worldometers.info/coronavirus/country/us/" target="_blank">Worldometers.info</a>, based in Dover, Delaware, U.S.A.</p>
        <p>The <a href="https://www.cdc.gov/coronavirus/2019-ncov/vaccines/faq.html" target="_blank">CDC</a> recommends that those recovered from COVID should still be vaccinated if given the chance. Since federal and state data sources do not disclose the number of vaccinated people who are also recovered from COVID, there is an overlap between recovered and vaccinated data. Since federal and state data sources do not disclose this overlap, and since there is no standard metric for what a recovered patient is, we are focusing solely on vaccinated data in our tracker. If data comes out regarding this overlap, we will add recovered cases back to the site.</p>
        <h2>About</h2>
        <p>This website was created by a few high school seniors from California. Data comes from state and federal sources. Thank you to Professor Lorene Nelson, PhD, MS, and Professor Steven Goodman, MD, MHS, PhD for their insight and contributions to our knowledge about the epidemiology of COVID-19. If you have any questions, feel free to email: <a href="mailto:hello@vaccineprogress.info" target="_blank">hello@vaccineprogress.info</a>.</p>
        <p class="caption text--secondary" style="font-size: 11px !important;">Built with &lt;/&gt; and Vue.js by <a href="https://github.com/BowenYin" target="_blank" style="color: inherit;">Bowen</a>; created by Jason, Sara, Claire.</p>
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
