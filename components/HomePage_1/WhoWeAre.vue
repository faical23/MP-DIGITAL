<template>
<div 
    class="Backgorund whoweare-top v-scroll-reveal" v-scroll-reveal.reset
>
  <div class="WhoWeAre">
      <h1>Who we are !</h1>
      <div class="WhoWeAre__Cards">
        <div class="WhoWeAre__CardLeft">
          <div class="Card">
              <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M0 0h24v24H0V0z" fill="none"/><path d="M22 9.24l-7.19-.62L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21 12 17.27 18.18 21l-1.63-7.03L22 9.24zM12 15.4l-3.76 2.27 1-4.28-3.32-2.88 4.38-.38L12 6.1l1.71 4.04 4.38.38-3.32 2.88 1 4.28L12 15.4z"/></svg>
                <h4>Boutique Approach</h4>
                <p>There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable.</p>
          </div>
      </div>
        <div class="WhoWeAre__CardMidle">
            <div class="Card">
                <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M0 0h24v24H0V0z" fill="none"/><path d="M22 9.24l-7.19-.62L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21 12 17.27 18.18 21l-1.63-7.03L22 9.24zM12 15.4l-3.76 2.27 1-4.28-3.32-2.88 4.38-.38L12 6.1l1.71 4.04 4.38.38-3.32 2.88 1 4.28L12 15.4z"/></svg>
                    <h4>Proven Experts</h4>
                    <p>There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable.</p>
            </div>
            <div class="Card">
                <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M0 0h24v24H0V0z" fill="none"/><path d="M22 9.24l-7.19-.62L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21 12 17.27 18.18 21l-1.63-7.03L22 9.24zM12 15.4l-3.76 2.27 1-4.28-3.32-2.88 4.38-.38L12 6.1l1.71 4.04 4.38.38-3.32 2.88 1 4.28L12 15.4z"/></svg>
                    <h4>Problem Solvers</h4>
                    <p>There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable.</p>
            </div>
        </div>
        <div class="WhoWeAre__CardRight">
            <div class="Card">
                <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M0 0h24v24H0V0z" fill="none"/><path d="M22 9.24l-7.19-.62L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21 12 17.27 18.18 21l-1.63-7.03L22 9.24zM12 15.4l-3.76 2.27 1-4.28-3.32-2.88 4.38-.38L12 6.1l1.71 4.04 4.38.38-3.32 2.88 1 4.28L12 15.4z"/></svg>
                    <h4>Growth Fuelers</h4>
                    <p>There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable.</p>
            </div>
        </div>
        </div>
  </div>
</div>

</template>

<script>


export default {
  layout: 'WhoWeAre',
  data() {
    return {
    }
  },


  components: {

  },

}

</script>

<style   scoped>

.WhoWeAre{
    width:80%;
    margin:30px auto;
    padding:100px 0px;
}
.Backgorund{
    width:80%;
    margin:30px auto;
    padding:100px 0px;
    background-image: url(../../assets/images/backgroudnCard.png);
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
}
.WhoWeAre h1{
    font-family: 'Poppins', sans-serif;
    font-size:40px;
    letter-spacing: 1px;
    font-weight: bolder;
    text-align: center;
    position: relative;
    bottom:130px;
}

.Card{
    box-shadow: 0px 0px 11px -6px black;
    background:rgb(255, 255, 255);
    border-radius: 20px;
    margin:20px 10px;
    text-align: center;
    padding:30px 20px;
    position: relative;
}
.Card svg{
    width: 40px;
    height:40px;
    fill:rgba(3,202,146,1);
    position: relative;
}
.Card h4{
    font-size: 22px;
    padding: 20px 0px;
    font-weight: bold;
    letter-spacing:1px;
    margin-bottom: 20px;
}
.Card h4::after{
        content: "";
        height: 2px;
        width: 90px;
        background-color: rgba(3,202,146,1);
        position: absolute;
        left: 38%;
        top: 40%;
}
.Card p{
    padding: 20px 0px;
    font-size: 16px;
    line-height:26px;
}
.WhoWeAre .WhoWeAre__Cards{
    width:90%;
    display:flex;
    align-items:center;
    margin:auto;

}
@media only screen and (max-width: 1440px) {
    .Backgorund{
        width:100%;
    }
    .WhoWeAre{
        width:90%;
    }
}
@media only screen and (max-width: 1024px) {
    .Backgorund{
        width:100%;
    }
    .WhoWeAre{
        width:100%;
    }
    .Card h4{
    margin-bottom: 0px;
    }
    .Card h4::after{
            top: 35%;
    }
}
@media only screen and (max-width: 768px) {
    .Backgorund{
        width:100%;
        background:none;
        padding: 0px;
    }
    .WhoWeAre .WhoWeAre__Cards{
        display:block;
    }
    .WhoWeAre h1{
    bottom:0px;
    }
    .Card{
        width:70%;
        margin: 20px auto;
    }
        .Card h4::after{
            top: 45%;
            left: 40%;
    }
}
@media only screen and (max-width: 560px) {
    .Card{
        width:90%;
    }
        .Card h4::after{
            top: 40%;
            left: 36%;
    }
}

</style>
