<template>
  <div class="Footer">
      <div class="Footer__Content">
            <div class="LogoAndIcons">
                <n-link to="/">
                    <img
                    class="logo"
                    src="~static/Logo-With.png"
                    alt="Mark Perez Digital"
                    />
                </n-link>
                <div class="FacebookLinkden">
                        <svg version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
                            viewBox="0 0 112.196 112.196" style="enable-background:new 0 0 112.196 112.196;" xml:space="preserve">
                        <g>
                            <circle style="fill:white;" cx="56.098" cy="56.098" r="56.098"/>
                            <path style="fill:rgb(5, 30, 139);" d="M70.201,58.294h-10.01v36.672H45.025V58.294h-7.213V45.406h7.213v-8.34
                                c0-5.964,2.833-15.303,15.301-15.303L71.56,21.81v12.51h-8.151c-1.337,0-3.217,0.668-3.217,3.513v7.585h11.334L70.201,58.294z"/>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        </svg>                   
                        <svg version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" x="0px" y="0px"
                            viewBox="0 0 112.196 112.196" style="enable-background:new 0 0 112.196 112.196;" xml:space="preserve">
                        <g>
                            <circle style="fill:#0cb887;" cx="56.098" cy="56.097" r="56.098"/>
                            <g>
                                <path style="fill:#F1F2F2;" d="M89.616,60.611v23.128H76.207V62.161c0-5.418-1.936-9.118-6.791-9.118
                                    c-3.705,0-5.906,2.491-6.878,4.903c-0.353,0.862-0.444,2.059-0.444,3.268v22.524H48.684c0,0,0.18-36.546,0-40.329h13.411v5.715
                                    c-0.027,0.045-0.065,0.089-0.089,0.132h0.089v-0.132c1.782-2.742,4.96-6.662,12.085-6.662
                                    C83.002,42.462,89.616,48.226,89.616,60.611L89.616,60.611z M34.656,23.969c-4.587,0-7.588,3.011-7.588,6.967
                                    c0,3.872,2.914,6.97,7.412,6.97h0.087c4.677,0,7.585-3.098,7.585-6.97C42.063,26.98,39.244,23.969,34.656,23.969L34.656,23.969z
                                    M27.865,83.739H41.27V43.409H27.865V83.739z"/>
                            </g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        <g>
                        </g>
                        </svg>
                </div>

            </div>
             <div class="Links">
                <a href="#"><p>What carry out a test? in the press</p></a>
                <a href="#"><p>About Us</p></a>
                <a href="#"><p>Press</p></a>
                <a href="#"><p>Associations</p></a>
                <a href="#"><p>Companies</p></a>
                <a href="#"><p>Individuals</p></a>
            </div>
            <div class="Email">
                <h2>Subscribe</h2>
                <form action="">
                    <input type="text" placeholder="Entrer email">
                    <button>Send</button>
                </form>
            </div>
      </div>
            <div class="RightReserved">
                <p>©2021-All right reserved</p>
                <p>Privacy Policy</p>
            </div>
  </div>
</template>

<script>


export default {
  layout: 'Footer',
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

.Footer{
    background-color:#2f485d;
    width:100%;
}
.Footer__Content{
    width:70%;
    margin:auto;
    display:flex;
    justify-content:space-between;
    padding:80px 0px;
    border-bottom:1px solid #dadada; ;
}
svg{
    width:40px;
    height:40px;
    margin:30px 5px;
    cursor: pointer;
}
p{
    color: #f8f8f8;
    padding:7px 0px;
    font-size: 16px;
}
.logo{
    max-width: 200px;
    max-height: 100px;
}
.LogoAndIcons{
    width:100%;
}
.Links,.Email{
    width:100%;
}
h2{
    color: #f8f8f8;
    font-family: 'Poppins', sans-serif;
    font-size:24px;
    letter-spacing: 1px;
    margin-bottom: 20px;
}
form{
    background-color:white;
    padding:10px;
    border-radius:5px;
}
input{
    padding:15px  5px;
    width:70%;
    border: none;
}
input:focus{
    border: none !important;
}
::placeholder{
    font-size: 19px;
    color: #dadada;
}
button{
    padding:10px 30px;
  letter-spacing: 1px;
  font-weight: 600;
  color: #fff;
  background-color: #00c790 !important;
  border:#00c790 !important;
  border-radius:50px;
  font-size: 18px;
  cursor: pointer;
}
p:hover{
    color: #00c790 ;
    color:rgb(5, 30, 139);
}
.RightReserved{
    width:70%;
    margin:auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 25px 0px;
}
@media only screen and (max-width: 1440px){
.Footer__Content,.RightReserved{
    width:85%;
}
}
@media only screen and (max-width: 1024px){
.Footer__Content,.RightReserved{
    width:90%;
}
input{
    width:60%;
}
}
/* @media only screen and (max-width: 768px){
.Footer__Content,.RightReserved{
    width:98%;
}
button{
    padding:4px 15px;
}
} */
@media only screen and (max-width: 768px){
.Footer__Content{
    width:100%;
    display: block;
    text-align: center;
}
form{
    width:80%;
    margin: 10px auto;
}

}
</style>
