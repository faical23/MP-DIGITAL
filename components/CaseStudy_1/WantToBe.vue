<template>
  <div class="WantToBe ">
      <h1>WANT TO BE OUR NEXT SUCCESS SRORY ?</h1>
      <p>Our track record proves we know how to help you make more money and fuel business growth</p>
      <button>REQUEST PROPOSAL</button>
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
.WantToBe{
    width:70%;
    border-radius:30px;
    margin: 300px auto 100px auto;
    padding:40px 30px ;
    text-align:center;
    background-image: url(../../assets/images/backgroundWant.png);
    background-position: center;
    background-repeat: no-repeat;
    background-size:cover;

}
h1{
font-size:35px;
  font-weight:bolder;
  color: white;
  font-family: 'Poppins', sans-serif;
}
p{
    font-size:25px;
    color: white;
    width:50%;
    margin: 20px auto;
}
button{
padding:15px 35px;
  letter-spacing: 1px;
  font-weight: bold;
  color: #fff;
  background-color: rgb(0,197,142) !important;
  border: none !important;
  font-size: 25px;
  border-radius:50px;
  margin-top:40px;
  cursor: pointer;
}
@media only screen and (max-width: 1440px) {
    .WantToBe{
        width:85%;
    }
}
@media only screen and (max-width: 1024px) {
    .WantToBe{
        width:95%;
    }
    p{
        width:80%;
    }
}
@media only screen and (max-width: 768px) {
    p{
        width:100%;
    }
}
@media only screen and (max-width: 560px) {
.WantToBe{
    margin:100px auto;
}
    p{
        font-size: 17px;
    }
    h1{
        font-size: 25px;
    }
    button{
        font-size: 20px;
    }
}
</style>
