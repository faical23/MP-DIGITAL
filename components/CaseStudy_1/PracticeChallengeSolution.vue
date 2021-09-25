<template>
  <div class="PracticeChallengeSolution ">
      <div class="Practice ">
          <div class="Practice__Content">
                <h1>PRIVATE PRACTICE INCREASES THIER LEAD BOLUME BY 68.04%</h1>
                <p>Dr. Ari Sytner is a passionate and highly-skilled therapist who focuses on relationship, dating, and marriage therapy.</p>
                <p>Based in New Jersey, Dr. Ari’s practice mainly services parts in
                and around Essex County, NJ as well as New York County, NY
                but with the ability to offer his services on a national basis.</p>
                                <p>Dr. Ari was an existing advertiser and wanted to further use
                Google Ads to be the main driving marketing channel for
                new clients.</p>
          </div>
          <div class="Practice__Illustrations">
            <img  src="../../assets/images/Illustrations/Practice.png" alt="">
          </div>
      </div>
      <div class="Practice Challenge PracticeZone ">
          <div class="Practice__Illustrations">
            <img  src="../../assets/images/Illustrations/Challange.png" alt="">
          </div>
          <div class="Practice__Content">
                <h1>CHALLENGE</h1>
                <p>Overtime, Dr. Ari noticed that the quantity and the quality of
                  leads had been decreasing and he needed to see an
                  increase in conversion volume and lead quality to
                  continue advertising.</p>
                <p>Dr. Ari’s practice was also unable to accept insurance and
                    priced themselves as a premium solution when compared
                      to the local competition, posing challenges for generating
                      qualified leads.</p>
                                <p>Dr Ari was running two campaigns, a local campaign as well
                  as a national campaign targeting select geographies. Both
                  campaigns had many, small, bid adjustments made over
                  the course of the campaigns running. </p>
                                                  <p>With so many small bid adjustments in different areas being
made in short periods of time, without enough data to
justify the changes, it was difficult to diagnose the exact
reasons why the campaigns started to slip in performance
and looked like a “death by a thousand cuts” situation.</p>
          </div>
      </div>
  <div class="Practice Challenge Solution  SolutionZone ">
          <div class="Practice__Illustrations">
            <img  src="../../assets/images/Illustrations/Solution.png" alt="">
          </div>
          <div class="Practice__Content">
                <h1>SOLUTION</h1>
                <p>The first step was to create a new local and a new national
campaign using the existing framework as our starting point,
without all of the additional bid adjustments in the old
campaigns..</p>
                <p>We also made improvements to the existing framework such
as creating new ads and adding more negative keywords to
the account.</p>
                                <p>Within just one month, we had seen some noteworthy
improvements: </p>
<div class="Arrows">
  <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M0 0h24v24H0V0z" fill="none"/><path d="M12 8l-6 6 1.41 1.41L12 10.83l4.59 4.58L18 14l-6-6z"/></svg>
    <h3>Conversion Rate Increased by 39.89%</h3>
</div>
<div class="Arrows">
  <svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="#000000"><path d="M24 24H0V0h24v24z" fill="none" opacity=".87"/><path d="M16.59 8.59L12 13.17 7.41 8.59 6 10l6 6 6-6-1.41-1.41z"/></svg>
  <h3>Cost Per Conversion Decreased by 12.68%</h3>
</div>
          </div>
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
.PracticeChallengeSolution{
    width: 70%;
    margin: 10px auto;
}
.Practice{
  display: flex;
  justify-content: space-between;
}
.Practice__Illustrations,.Practice__Content{
  width: 100%;
}
h1{
      font-family: 'Poppins', sans-serif;
    font-size: 38px;
    font-weight:bolder;
    margin-bottom:50px;
}
p{
    margin: 15px 0px;
    font-size: 20px;
    font-weight:600;
    color: #b4b4b4;
    width:85%;
}
.Practice__Content{
  position: relative;
  top: 100px;
}
.Challenge .Practice__Illustrations{
  position: relative;
  right: 100px;
  top: 150px;
}
.Solution{
  margin: 60px 0px !important;
}
.Arrows{
  display: flex;
  align-items: center;
  margin:20px 0px;
}
.Arrows h3{
      font-family: 'Poppins', sans-serif;
    font-size: 30px;
    font-weight:bolder;
    width:72%;
}
svg{
  width: 90px;
  height: 90px;
  border-radius:100%;
  background-color:rgb(0,197,142);
  fill:white;
  margin-right: 30px;
}
@media only screen and (max-width: 1440px) {
  .PracticeChallengeSolution{
    width: 80%;
}.Challenge .Practice__Illustrations{
  right: 40px;
  top:180px;
}
.Challenge .Practice__Content{
  left: 40px;
}
.Challenge p{
  width:100%;
}
}
@media only screen and (max-width: 1024px) {
  .PracticeChallengeSolution{
    width: 90%;
}
h1{
  font-size:28px;
}
p{
  width:90%;
  font-size: 16px;
}
}
@media only screen and (max-width: 768px) {
  svg{
    width:60px;
    height:60px;
  }
  .Arrows h3{
    font-size: 20px;
}
.Challenge,.Practice{
  align-items: center;
}

}
@media only screen and (max-width: 560px) {
.Challenge,.Practice{
  display:block;
  text-align: center;
}
.Practice__Content{
  position: relative;
  top: 0px;
  right:0px !important;
  left:0px !important;
  width:100%;
  margin: 50px auto !important;  
}
p{
    margin: 10px auto !important;  

}
.Challenge .Practice__Illustrations{
  right: 0px;
  top: 0px;
}
.PracticeZone,.SolutionZone{
  display: grid;
}
.PracticeZone .Practice__Illustrations ,.SolutionZone .Practice__Illustrations {
    order:1;
}

}
</style>
