<template>
  <div class="Reviews">
        <h1>Testimonial</h1>
        <div class="Reviews__Single v-scroll-reveal" v-scroll-reveal.reset>
            <div class="Reviews__Single__Img">
                <img src="../../assets/images/Reviews.png" alt="">
            </div>
            <div class="Reviews__Single__Content">
                    <div class="TitleAndReviews">
                            <h3 class="Titre">Amazing Service !</h3>
                            <h3 class="ReviewsNumber">{{Reviews[ReviewsWant].Rating}}<span>/5</span></h3>
                    </div>
                    <p>{{Reviews[ReviewsWant].Description}}</p>
                    <div class="Star">
                        <svg v-for="n in 5" :style=" Math.floor(Reviews[ReviewsWant].Rating) < n  ?  'fill: #c8c8c8' : 'fill:yellow '" :key='n'  xmlns="http://www.w3.org/2000/svg" enable-background="new 0 0 24 24" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><g><path d="M0,0h24v24H0V0z" fill="none"/><path d="M0,0h24v24H0V0z" fill="none"/></g><g><path d="M12,17.27L18.18,21l-1.64-7.03L22,9.24l-7.19-0.61L12,2L9.19,8.63L2,9.24l5.46,4.73L5.82,21L12,17.27z"/></g></svg>
                    </div>
                    <div class="NameAndSwitch">
                        <div class="Name" >
                            <h4>{{Reviews[ReviewsWant].Name}}</h4>
                            <span>{{Reviews[ReviewsWant].Status}}</span>
                        </div>
                        <div class="SwitchRow" >
                            <svg @click="SwitchToAnotherReviews('Back')"  :class="ReviewsWant > 0 ? 'ArrowActive' : '' "  xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M0 0h24v24H0V0z" fill="none" opacity=".87"/><path d="M17.51 3.87L15.73 2.1 5.84 12l9.9 9.9 1.77-1.77L9.38 12l8.13-8.13z"/></svg>
                            <svg @click="SwitchToAnotherReviews('Next')" :class="Reviews.length >(ReviewsWant+1) ? 'ArrowActive' : '' "  xmlns="http://www.w3.org/2000/svg" enable-background="new 0 0 24 24" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><g><path d="M0,0h24v24H0V0z" fill="none"/></g><g><polygon points="6.23,20.23 8,22 18,12 8,2 6.23,3.77 14.46,12"/></g></svg>
                        </div>
                    </div>
            </div>
        </div>
  </div>
</template>



<script>

export default {
  layout: 'Reviews',
  data() {
    return {
        ReviewsWant:0,
        Reviews:[
            {
                Img:'',
                Rating:3.75,
                Description:'At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi sint occaecati cupiditate non provident, similique sunt in culpa qui officia deserunt mollitia animi',
                Name:'Cherry Jac',
                Status:'CEO | Jaminak Saloon'
            },
            {
                Img:'',
                Rating:4.50,
                Description:'At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi sint occaecati cupiditate non provident, similique sunt in culpa qui officia deserunt mollitia animi',
                Name:'Faical bahsis',
                Status:'CEO | Jaminak Saloon'
            },
            {
                Img:'',
                Rating:5,
                Description:'At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti quos dolores et quas molestias excepturi sint occaecati cupiditate non provident, similique sunt in culpa qui officia deserunt mollitia animi',
                Name:'Ada lovelace',
                Status:'CEO | Jaminak Saloon'
            }
        ]
    }
  },
  components: {

  },
  methods: {
        SwitchToAnotherReviews(Condition){
            let ReviewsLength = this.Reviews.length
            let lengthSwitch =  this.ReviewsWant +1
                if(Condition == "Next" && ReviewsLength > lengthSwitch ){
                    this.ReviewsWant += 1
                }
                else if(Condition == "Back" && this.ReviewsWant > 0 ){
                    this.ReviewsWant -= 1
                    console.log(ReviewsLength)
                }
        }
  }

}

</script>

<style   scoped>

@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@600&display=swap');
.Reviews{
    width: 60%;
    margin: 100px auto;
}
.Reviews h1{
    font-family: 'Poppins', sans-serif;
    font-size:40px;
    letter-spacing: 1px;
    font-weight: bolder;
    text-align: center;
}
.Reviews__Single{
    display: flex;
    box-shadow: 0px 0px 11px -6px black;
    height:500px;
    margin:60px 0px;
}
.TitleAndReviews,.NameAndSwitch{
    display: flex;
    justify-content:space-between
}
.Reviews__Single__Img{
    width: 60%;
}
.Reviews__Single__Img img{
    width: 100%;
    height: 100%;
    object-fit: cover;
}
.Reviews__Single__Content{
    width:100%;
    padding:60px;
}
.Reviews__Single__Content h3,h4{
    font-family: 'Poppins', sans-serif;
    font-size:25px;
    letter-spacing: 1px;
    font-weight: bolder;
}
h4 {
    font-size:20px;
}

.TitleAndReviews{
    margin-bottom: 30px;
}
.Reviews__Single__Content .ReviewsNumber {
    color:#959595;
}
.Reviews__Single__Content span {
    font-size: 15px;
}
p{
        color:#959595;
        font-weight: 600;
        line-height:35px;
        font-size: 17px;
}
.Star svg{
    width:30px;
    height:30px;
    margin: 40px 0px;
    /* fill: yellow; */
}
.Name span{
    color:#959595;
    font-size: 18px;
}
.SwitchRow svg{
    width:40px;
    height:40px;
    border: 1px solid #959595;
    border-radius: 100%;
    padding:4px;
    margin:0px 2px;
    fill: #959595;
}
.ArrowActive{
    border: 1px solid #00c790 !important;
    fill: #00c790 !important;
    cursor: pointer;
}
@media only screen and (max-width: 1440px) {
    .Reviews{
        width: 70%;
    }
}
@media only screen and (max-width: 1024px) {
    .Reviews{
        width: 80%;
    }
    .Reviews__Single__Content{
        padding:30px;
    }
    .Reviews__Single__Img{
        width: 80%;
    }
}
@media only screen and (max-width: 768px) {
    .Reviews{
        width: 95%;
    }
    p{
        font-size:15px;
        line-height:30px;
    }

}
@media only screen and (max-width: 560px) {
    .Reviews__Single{
        display: block;
        height:auto;
    }
    .Reviews__Single__Img{
        width: 100%;
    }

}
</style>