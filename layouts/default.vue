<template>
  <div>
    <app-nav> </app-nav>
    <nuxt />

    <!-- <app-footer></app-footer> -->
  </div>
</template>

<script>
import Nav from '@/components/Nav.vue'
import Footer from '@/components/Footer.vue'

export default {
  computed: {
    getPath() {
      return this.$route.fullPath
    }
  },
  components: {
    'app-nav': Nav,
    'app-footer': Footer
  }
}
</script>
