<template>
  <div class="WantToBe  v-scroll-reveal" v-scroll-reveal.reset >
      <div class="Content">
                  <h1>Want To Be Our Next Success Story?</h1>
                <p>There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable.</p>
      </div>
      <div class="proposal">
                  <button>Request Proposal</button>
      </div>

  </div>
</template>

<script>


export default {
  layout: 'WantToBe',
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
.WantToBe{
    width:60%;
    background-color:rgb(0, 255, 170);
    background: linear-gradient(#00eeac, #00c68f);
    margin:0px auto;
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:40px 40px;
    border-radius:10px;
    position: relative;
    bottom: 154px;
}
h1{
    font-family: 'Poppins', sans-serif;
    font-size:30px;
    letter-spacing: 1px;
    font-weight: bolder;
    color:white;
    padding-bottom: 30px;
}
p{
    color:white;
    font-size:17px;
    line-height:30px;
    width: 90%;
}
.Content{
    width:60%;
}
.proposal{
    width:40%;
    text-align: -webkit-right;
    text-align: end;
}
button{
    padding:20px 30px;
  letter-spacing: 1px;
  color: #fff;
  background-color: #2f495e !important;
  border:#2f495e !important;
  border-radius:50px;
  font-size: 20px;
}
@media only screen and (max-width: 1440px){
  .WantToBe{
    width: 80%;
  }
}
@media only screen and (max-width: 1024px){
  .WantToBe{
    width: 95%;
  }
  h1{
    font-size:25px;
    }

}
@media only screen and (max-width: 1024px){
  .WantToBe{
    bottom: 50px;
  }
  h1{
    font-size:20px;
    }
    p{
        font-size:15px
    }

}
@media only screen and (max-width: 560px){
  .WantToBe{
    display:block;
    text-align:center;
  }
  .Content,.proposal{
      width: 100%;
      text-align: center !important;
  }
  button{
      margin: 30px 0px;
  }

}
</style>
