<template>
  <div>
      <Hero/>
      <Statisqtique/>
      <Card/>
      <AboutUs/>
      <WhoWeAre/>
      <WantTobeOur/>
      <ContactUs/>
      <Testimonial/>
      <Sponsore/>
      <Footer/>

  </div>
</template>

<script>

import Hero from '@/components/HomePage/Hero.vue'
import Statisqtique from '@/components/HomePage/Statistique.vue'
import Card from '@/components/HomePage/Card.vue'
import AboutUs from '@/components/HomePage/AboutUs.vue'
import WhoWeAre from '@/components/HomePage/WhoWeAre.vue'
import ContactUs from '@/components/HomePage/ContactUs.vue'
import Testimonial from '@/components/HomePage/Testimonial.vue'
import Sponsore from '@/components/HomePage/Sponsore.vue'
import Footer from '@/components/NewFooter.vue'
import WantTobeOur from '@/components/HomePage/WantTobeOur.vue'



export default {
  layout: 'homepage',
  data() {
    return {
    }
  },


  components: {
    Hero,
    Statisqtique,
    Card,
    AboutUs,
    WhoWeAre,
    ContactUs ,
    Testimonial,
    Sponsore,
    Footer,
    WantTobeOur
  },

}

</script>

<style   scoped>

</style>
