<template>
  <div class="ContactUs v-scroll-reveal" v-scroll-reveal.reset>
      <div class="ContactUs__Ilustration">
        <img class="Heroillustration" src="../../assets/images/Illustrations/HomePgae4.png" alt="">
      </div>
    <div class="ContactUs__Content">
            <h1>Contact Us</h1>
            <form 
                  @submit="handleRequest"
                  action="https://formspree.io/info@markperez.dev"
                  method="POST"
                  >
                <input 
          type="text"
          name="name"
          placeholder="Name"
          aria-label="full name"
          required>
                <input 
          type="email"
          name="email"
          placeholder="Email"
          aria-label="email address"
          required>
                <textarea 
            class="textarea"
            name="message"
            placeholder="Message..."
            aria-label="message"
            required></textarea>
                <button class="button buttonPrimary is-rounded" value="submit">Submit</button>
            </form>
      </div>
  </div>
</template>

<script>


export default {
  layout: 'ContactUs',
  data() {
    return {
    }
  },


  components: {

  },

}

</script>

<style   scoped>


@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@600&display=swap');
.ContactUs{
    width:70%;
    margin: 40px auto;
    display:flex;
}
.ContactUs__Ilustration,.ContactUs__Content{
    width:100%;
}
.ContactUs__Content{
    position: relative;
    top: 20px;
    left:10px;
}
.ContactUs__Content h1{
    font-family: 'Poppins', sans-serif;
    font-size:40px;
    padding-bottom: 40px;
    letter-spacing: 1px;
    font-weight: bold;
}
.buttonPrimary {
  padding:5px 30px;
  letter-spacing: 1px;
  font-weight: bold;
  color: #fff;
  background-color: #2f495e !important;
  border:#2f495e !important;
  margin:20px 0px;
}
.ContactUs input, .ContactUs textarea{
    display: block;
    width: 100%;
    padding:20px 25px;
    border-radius: 6px;
    margin-bottom:20px;
    border: 1px solid #c0c0c0;
    font-size:20px ;
}
::placeholder{
    color:#c0c0c0ef;
}
textarea{
    height:200px;
}

@media only screen and (max-width: 1440px){
  .ContactUs{
    width: 80%;
  }
}
@media only screen and (max-width: 1024px){
  .ContactUs{
    width: 100%;
  }

}
@media only screen and (max-width: 768px){
  .ContactUs{
    align-items: center;
  }
}
@media only screen and (max-width: 560px){
  .ContactUs{
    display:block;
    text-align: center;
  }
  .ContactUs input, .ContactUs textarea{
    width: 90%;
    margin:10px auto;
}
}
</style>
