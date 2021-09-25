<template>
  <div>
      <Hero/>
      <Number/>
      <Card/>
      <AboutUs/>
      <WoweAre/>
      <WantTobe/>
      <ContactUs/>
      <Testimonial/>
      <Sponsore/>
  </div>
</template>

<script>

import Hero from '@/components/HomePage_1/Hero.vue'
import Number from '@/components/HomePage_1/Numbers.vue'
import AboutUs from '@/components/HomePage_1/AboutUs.vue'
import Card from '@/components/HomePage_1/Card.vue'
import WoweAre from '@/components/HomePage_1/WhoWeAre.vue'
import WantTobe from '@/components/HomePage_1/WantTobeOur.vue'
import ContactUs from '@/components/HomePage_1/ContactUs.vue'
import Testimonial from '@/components/HomePage_1/Testimonial.vue'
import Sponsore from '@/components/HomePage_1/Sponsore.vue'

import gql from 'graphql-tag'

const articles = gql`
  {
    allBlog_postss {
      totalCount
    }
  }
`

export default {
  layout: 'homepage',
  data() {
    return {
      title: 'SEO for Beauty Brands',
      description:
        'MP Digital is a well-versed SEO Agency empowering beauty salons to be 1st-choice within their region.'
    }
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
          content: 'https://markperez.dev' + this.$route.fullPath
        },
        {
          hid: 'og:image', // open graph image
          property: 'og:image',
          content: 'https://markperez.dev/mp-digital-logo-dark.png'
        }
      ]
    }
  },

  components: {
     Hero,
     Number,
     AboutUs,
     Card ,
     WoweAre,
     WantTobe,
     ContactUs,
     Testimonial,
     Sponsore
  },

  apollo: {
    allBlog_postss: {
      query: articles,
      fetchPolicy: 'cache-and-network'
    }
  }
}
</script>

<style scoped>

</style>
