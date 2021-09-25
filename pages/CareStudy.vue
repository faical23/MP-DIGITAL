<template>
  <div>
      <u-animate-container>
    <u-animate
      name="fadeInDown"
      delay="0s"
      duration=".7s"
      :iteration="1"
      :offset="0"
      animateClass="animated"
      :begin="false" 
    >
    <Hero/>

    </u-animate>
      </u-animate-container>
      <u-animate-container>
    <u-animate
      name="fadeInDown"
      delay="0s"
      duration="1s"
      :iteration="2"
      :offset="0"
      animateClass="animated"
      :begin="true" 
    >
    <IncreasedLead/>

    </u-animate>
      </u-animate-container>
      <u-animate-container>
    <u-animate
      name="fadeInDown"
      delay="0s"
      duration=".7s"
      :iteration="3"
      :offset="0"
      animateClass="animated"
      :begin="true" 
    >
    <DoYouLikeMoney/>

    </u-animate>
      </u-animate-container>
      
    <PracticeChallengeSolution/>
    <WantToBe/>
    <Footer/>

  </div>
</template>

<script>

import Hero from '@/components/CareStudy/Hero.vue'
import IncreasedLead from '@/components/CareStudy/IncreasedLead.vue'
import DoYouLikeMoney from '@/components/CareStudy/DoYouLikeMoney.vue'
import PracticeChallengeSolution from '@/components/CareStudy/PracticeChallengeSolution.vue'
import WantToBe from '@/components/CareStudy/WantToBe.vue'
import Footer from '@/components/NewFooter.vue'


import Vue from 'vue'
import VueWow from 'vue-wow'
 import {UAnimateContainer, UAnimate} from 'vue-wow'

// mount with global
Vue.use(VueWow)
 
 import 'animate.css'
export default {
  layout: 'homepage',
  data() {
    return {
    }
  },


  components: {
    Hero,
    IncreasedLead,
    DoYouLikeMoney,
    PracticeChallengeSolution,
  WantToBe,
  Footer,
      UAnimateContainer,
    UAnimate
  },

}

</script>

<style   scoped>

</style>
