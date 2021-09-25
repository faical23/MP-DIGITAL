<template>
  <div class="DoYouLike  v-scroll-reveal" v-scroll-reveal.reset>
        <div class="Illustrations">
            <img  src="../../assets/images/Illustrations/CaseStudyIllustartion1.png" alt="">
        </div>
        <div class="Content">
                <h3>quick question:</h3>
                <h1 class="Green">Do You Like <span>Money</span> ?</h1>
                <p>Then you'll love our content.</p>
                <form 
                  class="f_subscribe_two mailchimp validate"
                  action="https://dev.us20.list-manage.com/subscribe/post?u=0e646f9cc09aa7c7a450ae8b6&amp;id=a5dd106a2e"
                  method="post"
                  id="mc-embedded-subscribe-form"
                  name="mc-embedded-subscribe-form"
                  target="_blank"
                  novalidate>
                    <input type="text" placeholder="Email*">
                    <button>Submit</button>
                </form>
        </div>
  </div>
</template>

<script>
export default {
  computed: {

  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@600&display=swap');
.DoYouLike{
    width: 70%;
    display: flex;
    justify-content: space-between;
    margin: 120px auto 20px auto;
}
.Illustrations,.Content{
    width: 100%;
}
.Content{
    position: relative;
    top: 100px;
    left: 40px;
}
h3{
    font-size:25px;
    font-weight:bolder;
    margin-bottom: 10px;
}
h1{
    font-family: 'Poppins', sans-serif;
    font-size: 35px;
    font-weight:bolder;
    color: rgb(0,197,142);

}
span{
    color: #2f495e;
}
p{
    margin: 30px 0px;
    font-size: 18px;
}
input{
    display: block;
    width: 90%;
    padding:15px 25px;
    border-radius: 6px;
    margin-bottom:20px;
    border: 1px solid #c0c0c0;
    font-size:20px ;
}
button{
    padding:12px 35px;
    letter-spacing: 1px;
    font-weight: bold;
    color: #fff;
    background-color: #2f495e !important;
    border:#2f495e !important;
    margin:20px 0px;
    border-radius:50px;
    font-size:20px;
    cursor: pointer;
}
@media only screen and (max-width: 1440px) {
    .DoYouLike{
        width: 80%;
    }
    .Content{
    top: 60px;
}
}
@media only screen and (max-width: 1024px) {
    .DoYouLike{
        width: 90%;
    }
    .Content{
    top: 20px;
    }
}
@media only screen and (max-width: 768px) {
    .Content{
    top: 0px;
    }
    h1{
    font-size: 25px;

}
}
@media only screen and (max-width: 560px) {
    .DoYouLike{
        width: 100%;
        text-align: center;
        display:block
    }
    .Content{
    left: 0px;
    }
    input{
        margin: 0px auto;
    }
}

</style>
