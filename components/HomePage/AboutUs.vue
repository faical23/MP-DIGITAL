<template>
  <div class="AboutUs">
      <div class="AboutUs__Ilustration">
        <img class="Heroillustration" src="../../assets/images/Illustrations/HomepageUlli1.png" alt="">
      </div>
    <div class="AboutUs__Content">
            <h1>About Us</h1>
            <p>It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters, as opposed to using 'Content here, content here', making it look like readable English. Many desktop publishing packages and web page editors now use Lorem Ipsum as their default model text, and a search for 'lorem ipsum' will uncover many web sites still in their infancy. Various versions have evolved over the years, sometimes by accident, sometimes on purpose (injected humour and the like)</p>
      </div>
  </div>
</template>

<script>


export default {
  layout: 'AboutUs',
  data() {
    return {
    }
  },


  components: {

  },

}

</script>

<style   scoped>
/* @font-face {
  font-family: 'Popping-Bold';
  src: url('https://fonts.googleapis.com/css2?family=Poppins:wght@500&display=swap');;
} */

@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@600&display=swap');
.AboutUs{
    width:70%;
    margin: 20px auto;
    display:flex;
}
.AboutUs__Ilustration,.AboutUs__Content{
    width:100%;
}
.AboutUs__Content{
    position: relative;
    top: 20px;
    left:10px;
}
.AboutUs__Content h1{
    font-family: 'Poppins', sans-serif;
    font-size:40px;
    padding-bottom: 30px;
    letter-spacing: 1px;
    font-weight: bolder;
}
.AboutUs__Content p{
    font-size:18px;
    line-height:30px;
    color: #797979;
    width:90%;
}
@media only screen and (max-width: 1440px){
  .AboutUs{
    width: 80%;
  }
  .AboutUs__Content p{
    font-size:17px;
    width:90%;
  }
}
@media only screen and (max-width: 1024px){
  .AboutUs{
    width: 100%;
  }
  .AboutUs__Content p{
    font-size:16px;
    width:95%;
  }
}
@media only screen and (max-width: 768px){
  .AboutUs{
    align-items: center;
  }
}
@media only screen and (max-width: 560px){
  .AboutUs{
    display:block;
    text-align: center;
  }
}

</style>
