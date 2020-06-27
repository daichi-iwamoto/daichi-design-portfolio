<template>
  <div class="container">
    <div id="ladies">
      <Header />
      <Mainv />
      <Section01 />
      <Section02 />
      <Section03 />
      <Footer />
      <Load />
    </div>
  </div>
</template>

<script>
import Header from '~/components/Header.vue'
import Footer from '~/components/Footer.vue'
import Load from '~/components/ladies/Load.vue'
import Mainv from '~/components/Mainv.vue'
import Section01 from '~/components/Section01.vue'
import Section02 from '~/components/Section02.vue'
import Section03 from '~/components/Section03.vue'

export default {
  components: {
    Header,
    Load,
    Mainv,
    Section01,
    Section02,
    Section03,
    Footer
  }
}
</script>
