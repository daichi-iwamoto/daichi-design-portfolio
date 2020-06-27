<template>
  <header id="header">
    <div class="header_logo">
      <p class="header_logo-txt">
        design
        <br>portfolio
      </p>
      <div class="header_logo-mode">
        <nuxt-link to="/mens/" class="header_logo-modeLink active">
          for mens
        </nuxt-link>
        <nuxt-link to="/ladies/" class="header_logo-modeLink">
          for ladies
        </nuxt-link>
      </div>
    </div>
    <div class="header_links">
      <nuxt-link v-scroll-to="'#section01'" to class="header_links-link">
        Sec1
      </nuxt-link>
      <nuxt-link v-scroll-to="'#section02'" to class="header_links-link">
        Sec2
      </nuxt-link>
      <nuxt-link v-scroll-to="'#section03'" to class="header_links-link">
        Sec3
      </nuxt-link>
    </div>
  </header>
</template>
