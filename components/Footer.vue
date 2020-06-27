<template>
  <footer id="footer">
    <div class="footer_links">
      <nuxt-link v-scroll-to="'#section01'" to class="footer_links-link">
        Sec1
      </nuxt-link>
      <nuxt-link v-scroll-to="'#section02'" to class="footer_links-link">
        Sec2
      </nuxt-link>
      <nuxt-link v-scroll-to="'#section03'" to class="footer_links-link">
        Sec3
      </nuxt-link>
    </div>
    <div class="footer_logo">
      <p class="footer_logo-txt">
        design
        <br>portfolio
      </p>
    </div>
  </footer>
</template>
