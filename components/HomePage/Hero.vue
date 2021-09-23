<template>
  <div>
    <!-- assign your video to the following class below -->
      <!-- navbar put manually for customization -->
    <section class="Hero">
      <nav class="Navbar HomePageNav">
        <div class="navbar-brand">
          <n-link class="navbar-item" to="/">
            <img
              class="logo"
              src="~static/Logo-With.png"
              alt="Mark Perez Digital"
            />
          </n-link>

          <!-- Navbar Burger -->
          <span
            class="navbar-burger"
            @click="showNav = !showNav"
            data-target="navMenu"
          >
            <span></span>
            <span></span>
            <span></span>
          </span>
        </div>

        <!-- Navbar Menu -->
        <div id="navMenu" class="navbar-menu" :class="{ 'is-active': showNav }">
          <div @click="showNav = !showNav" class="navbar-end">
            <n-link class="navbar-item" to="/blog/">Blog</n-link>
            <n-link class="navbar-item" to="/gear/">Gear</n-link>
            <n-link class="navbar-item" to="/contact/">Contact</n-link>
            <svg  xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M0 0h24v24H0V0z" fill="none"/><path d="M15.5 14h-.79l-.28-.27C15.41 12.59 16 11.11 16 9.5 16 5.91 13.09 3 9.5 3S3 5.91 3 9.5 5.91 16 9.5 16c1.61 0 3.09-.59 4.23-1.57l.27.28v.79l5 4.99L20.49 19l-4.99-5zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z"/></svg>
            <a
              class="navbar-item"
              target="_blank"
              href="https://calendly.com/info-30250/discovery-call"
              ><button class="button  buttonPrimary is-rounded">Book a Call</button></a
            >
          </div>
        </div>
      </nav>
      
        <img class="RightPointHeroGlobal" src="../../assets/images/Illustrations/PointHeroHomePage.png" alt="">
          <div class="Hero__Content">
            <div class="Hero__Content__Text">
                <h1>MP DIGITAL</h1>
                <p>It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters, as opposed to using 'Content here, content here', making it look like readable English. </p>
                  <a
                    class="navbar-item"
                    target="_blank"
                    href="https://calendly.com/info-30250/discovery-call"
                    ><button class="button buttonPrimary is-rounded">Book a Call</button></a
                  >     
                 </div>
            <div class="Hero__Content__Illustration">
                <img class="Heroillustration" src="../../assets/images/Illustrations/HeroHomePage.png" alt="">
                <img class="RightPointHero" src="../../assets/images/Illustrations/PointHeroHomePage.png" alt="">
            </div>
          </div>
      </section>
    <!-- <app-portfolio></app-portfolio> -->
  </div>
</template>

<script>
import Portfolio from '@/components/Portfolio.vue'
import NavHome from '@/components/NavHome.vue'
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
      showNav: false,
      title: 'MP Digital',
      description:
        'MP Digital is a well-versed SEO Agency empowering beauty salons to be 1st-choice within their region.'
    }
  },

  head() {
    return {
      title: 'SEO for Beauty Salons',
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
          content:
            'https://markperez.dev/mp-digital-logo-dark.png'
        }
      ]
    }
  },

  components: {
    'app-portfolio': Portfolio,
    'app-navhome': NavHome
  },

  apollo: {
    allBlog_postss: {
      query: articles,
      fetchPolicy: 'cache-and-network'
    }
  }
}

</script>

<style   scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@600&display=swap');
.Hero{
  width: 90%;
  margin:auto;
  border-radius: 20px;
  margin-top: 20px;
  background: rgb(0,197,142);
  background: linear-gradient(90deg, rgb(12 223 164) 0%, rgba(3,202,146,1) 36%, rgba(11,222,162,1) 65%, rgb(40, 255, 194) 80%);
}
.HomePageNav{
    padding:20px 140px 40px 140px;
    display: flex;
    justify-content:space-between;
}
.navbar-item {
    font-size: 18px;
    padding-right: 2rem;
    color: white;
    font-weight: bolder;
}
.Navbar  svg{
    fill: white ;
    margin: 0px 10px !important;
}
.navbar-item:hover {
  color: #2f495e;
}
 .Hero__Content{
  display: flex;
  justify-content:space-between;
  padding:40px 140px;
}
.Hero__Content__Text{
  width:80%;
  position: relative;
  /* left: 50px; */
  top:20px;
}
.navbar-end {
    display: flex;
    align-items: center;
}
.logo {
  max-height: 3rem;
}
.Hero__Content__Text h1{
  font-size:120px;
  font-weight:bolder;
  color: white;
  font-family: 'Poppins', sans-serif;
  text-shadow: 2px 2px 13px rgba(0, 0, 0, 0.726);
}
.Hero__Content__Text p{
  font-size:18px; 
  line-height:30px;
  color:white;
  width:100%;  

}
a:hover,
a:active,
a:focus {
  background-color: transparent;
  border:#2f495e transparent;
}

.buttonPrimary {
  padding:0px 20px;
  letter-spacing: 1px;
  font-weight: bold;
  color: #fff;
  background-color: #2f495e !important;
  border:#2f495e !important;
}

.Hero__Content__Text button{
  position: relative;
  top: 10px;
}
.Hero__Content__Illustration {
    position: relative;
      width:90%;
}
.Hero__Content__Illustration .Heroillustration{
      position: relative;
      left: 70px;
      bottom: 50px;
      z-index: 20;
}
.RightPointHero{
  width:300px;
  position: absolute !important;
  right:-50px;
  bottom:100px;
  z-index: 10;
  }
  .RightPointHeroGlobal{
    width:300px;
    position: absolute !important;
    left:60px ;
    bottom:70px ;
  }

@media only screen and (max-width: 1440px) {
  .Hero__Content__Text h1{
    font-size:80px;
  }
  .Hero__Content__Text{
    top:-30px;
  }
  .RightPointHeroGlobal{
    width:200px;
    bottom:0px ;
  }
  .RightPointHero{
    width:200px;
    
    /* right:-80px ; */
  }
}
@media only screen and (max-width: 1024px) {
  .HomePageNav{
    padding:20px 40px 40px 40px;
}
 .Hero__Content{
  padding:40px 40px;
}
  .Hero__Content__Text h1{
    font-size:50px;
  }
  .Hero__Content__Text p{
    font-size:14px;
    line-height:25px;
  }
  .Hero__Content__Illustration {
      width:100%;
  }
 .RightPointHeroGlobal{
    width:200px;
    top:500px ;
    left:40px;
  }
}
@media only screen and (max-width: 834px) {
  .HomePageNav{
    display:block;
  }
  .navbar-item,svg {
    color: #2f495e;
    fill: #2f495e !important;
  }
  svg {
    fill: #2f495e !important;
  }
  .navbar-end {
      display: block;
  }
  .Hero__Content__Text h1{
    font-size:40px;
  }
  .Hero__Content__Text p{
    font-size:13px;
    line-height:20px;
  }
  .Hero__Content__Illustration .Heroillustration{
      left: 30px;
  }
  .RightPointHero{
    width:150px;
    right:-20px;
  }
  .RightPointHeroGlobal{
    width:150px;
    top:420px;
  }
  .Hero__Content__Text{
  top:-40px;
}
.Hero__Content{
  padding:10px 40px;
}

}
@media only screen and (max-width: 560px) {
    .HomePageNav{
    padding:20px 5px 40px 5px;
  }
  .Hero__Content{
    padding:5px 5px;
    display:block;
    width:100%;
    text-align:center;
  }
  .Hero__Content__Text{
    width:100%;
  }
   .RightPointHeroGlobal,.RightPointHero{
     display:none;
  }
  .Hero__Content__Illustration .Heroillustration{
      margin:20px 0px;
      left: 0px;
      bottom: 0px;
}
}

</style>
