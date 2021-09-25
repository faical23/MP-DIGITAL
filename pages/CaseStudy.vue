<template>
  <div>
    <Hero/>
    <IncreasedLead/>
    <DoYouLikeMoney/> 
    <PracticeChallengeSolution/>
    <WantToBe/>
  </div>
</template>


<script>
import Hero from '@/components/CaseStudy_1/Hero.vue'
import IncreasedLead from '@/components/CaseStudy_1/IncreasedLead.vue'
import DoYouLikeMoney from '@/components/CaseStudy_1/DoYouLikeMoney.vue'
import PracticeChallengeSolution from '@/components/CaseStudy_1/PracticeChallengeSolution.vue'
import WantToBe from '@/components/CaseStudy_1/WantToBe.vue'
export default {
  data() {
    return {
      title: 'Contact',
      description:
        'Feel free to contact and send us an email. We will get back to them in no time!'
    }
  },
  
  components: {
    Hero,
    IncreasedLead,
    DoYouLikeMoney,
    PracticeChallengeSolution,
    WantToBe,
  },

  head() {
    return {
      title: this.title,
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: this.description
        },
        {
          hid: 'og:type', // open graph type
          property: 'og:type',
          content: 'website'
        },
        {
          hid: 'apple-mobile-web-app-title', // open graph mobile web app title
          name: 'apple-mobile-web-app-title',
          content: this.title
        },
        {
          hid: 'og:title', // open graph title
          property: 'og:title',
          content: this.title
        },
        {
          hid: 'og:description', // open graph description
          property: 'og:description',
          content: this.description
        },
        {
          hid: 'og:url', // open graph url
          property: 'og:url',
          content: 'https://markperez.dev' + this.$route.fullPath + '/'
        },
        {
          hid: 'og:image', // open graph image
          property: 'og:image',
          content:
            'https://markperez.dev/mp-digital-logo-dark.png'
        }
      ]
      
    }
  }
}
</script>

<style scoped>

</style>
