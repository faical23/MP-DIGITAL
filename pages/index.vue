<template>
  <div>
      <Hero/>
      <Statisqtique/>
      <Card/>

  </div>
</template>

<script>

import Hero from '@/components/HomePage/Hero.vue'
import Statisqtique from '@/components/HomePage/Statistique.vue'
import Card from '@/components/HomePage/Card.vue'



export default {
  layout: 'homepage',
  data() {
    return {
    }
  },


  components: {
    Hero,
    Statisqtique,
    Card
  },

}

</script>

<style   scoped>

</style>
