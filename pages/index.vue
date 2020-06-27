<template>
  <div class="container">
    <div>
      <Header />
      <Load />
    </div>
  </div>
</template>

<script>
import Header from '~/components/Header.vue'
import Load from '~/components/mens/Load.vue'

export default {
  components: {
    Header,
    Load
  }
}
</script>
