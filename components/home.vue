<template> 
    <div class="main">
      <div class="header">
        <h1>Shopping Website.</h1>
        <router-link to="/cart"><img src="./assets/cartCheck.png"></router-link>
      </div>
      <h1 class="title">sneakers</h1>
      <div class="sneakers">
        <div class="selct1" v-on:mouseover="hoverOn1" v-on:mouseleave="hoverOff1">
          <img class="slct-img1" src="./assets/Dsneaks1.png" alt="sneakers selection">
          <div class="addtoCart" v-if="visible1" > 
            <div class="text"><router-link to="/cart">add to cart <span>N25</span> </router-link></div>
          </div>
          <p>Lorem</p>
        </div>
        <div class="selct2" v-on:mouseover="hoverOn2" v-on:mouseleave="hoverOff2">
          <img class="slct-img2" src="./assets/Dsneaks2.png" alt="sneakers selection">
          <div class="addtoCart" v-if="visible2"> 
            <div class="text"><router-link to="/cart">add to cart <span>N25</span> </router-link></div>
          </div>
          <p>Lorem</p>
        </div>
        <div class="selct3" v-on:mouseover="hoverOn3" v-on:mouseleave="hoverOff3">
          <img class="slct-img3" src="./assets/Dsneaks3.png" alt="sneakers selection">
          <div class="addtoCart" v-if="visible3" > 
            <div class="text"><router-link to="/cart">add to cart <span>N25</span> </router-link></div>
          </div>
          <p>Lorem</p>
        </div>
      </div>

      <h1 class="title">jackets</h1>
      <div class="jackets">
        <div class="selct1" v-on:mouseover="hoverOn4" v-on:mouseleave="hoverOff4">
          <img class="slct-img1" src="./assets/Djacket1.png" alt="jackets selection">
          <div class="addtoCart" v-if="visible4" > 
            <div class="text"><router-link to="/cart">add to cart <span>N55</span> </router-link></div>
          </div>
          <p>Lorem</p>
        </div>
        <div class="selct2" v-on:mouseover="hoverOn5" v-on:mouseleave="hoverOff5">
          <img class="slct-img2" src="./assets/Djacket2.png" alt="jackets selection">
           <div class="addtoCart" v-if="visible5" > 
           <div class="text"><router-link to="/cart">add to cart <span>N65</span> </router-link></div>
          </div>
          <p>Lorem</p>
        </div>
        <div class="selct3" v-on:mouseover="hoverOn6" v-on:mouseleave="hoverOff6">
          <img class="slct-img3" src="./assets/Djacket3.png" alt="jackets selection">
           <div class="addtoCart" v-if="visible6" > 
           <div class="text"><router-link to="/cart">add to cart <span>N85</span> </router-link></div>
          </div>
          <p>Lorem</p>
        </div>
      </div>

      <h1 class="title">hats</h1>
      <div class="hats">
        <div class="selct1" v-on:mouseover="hoverOn7" v-on:mouseleave="hoverOff7">
          <img class="slct-img1" src="./assets/Dhat1.png" alt="hats selection">
          <div class="addtoCart" v-if="visible7" > 
            <div class="text"><router-link to="/cart">add to cart <span>N25</span> </router-link></div>
          </div>
          <p>Lorem</p>
        </div>
        <div class="selct2" v-on:mouseover="hoverOn8" v-on:mouseleave="hoverOff8">
          <img class="slct-img2" src="./assets/Dhat2.png" alt="hats selection">
          <div class="addtoCart" v-if="visible8" > 
           <div class="text"><router-link to="/cart">add to cart <span>N45</span> </router-link></div>
          </div>
          <p>Lorem</p>
        </div>
        <div class="selct3" v-on:mouseover="hoverOn9" v-on:mouseleave="hoverOff9">
          <img class="slct-img3" src="./assets/Dhat3.png" alt="hats selection">
          <div class="addtoCart" v-if="visible9" > 
           <div class="text"><router-link to="/cart">add to cart <span>N25</span> </router-link></div>
          </div>
          <p>Lorem</p>
        </div>
      </div>


      <h1 class="title">Men</h1>
      <div class="men">
        <div class="selct1" v-on:mouseover="hoverOn10" v-on:mouseleave="hoverOff10">
          <img class="slct-img1" src="./assets/Dmen1.png" alt="men selection">
          <div class="addtoCart" v-if="visible10" > 
           <div class="text"><router-link to="/cart">add to cart <span>N25</span> </router-link></div>
          </div>
          <p>Lorem</p>
        </div>
        <div class="selct2" v-on:mouseover="hoverOn11" v-on:mouseleave="hoverOff11">
          <img class="slct-img2" src="./assets/Dmen2.png" alt="men selection">
          <div class="addtoCart" v-if="visible11" > 
            <div class="text"><router-link to="/cart">add to cart <span>N50</span> </router-link></div>
          </div>
          <p>Lorem</p>
        </div>
        <div class="selct3" v-on:mouseover="hoverOn12" v-on:mouseleave="hoverOff12">
          <img class="slct-img3" src="./assets/Dmen3.png" alt="men selection">
          <div class="addtoCart" v-if="visible12" > 
            <div class="text"><router-link to="/cart">add to cart <span>N75</span> </router-link></div>
          </div>
          <p>Lorem</p>
        </div>



      </div>

      <h1 class="title">women</h1>
      <div class="women">
        <div class="selct1" v-on:mouseover="hoverOn13" v-on:mouseleave="hoverOff13">
          <img class="slct-img1" src="./assets/Dwomen1.png" alt="women selection">
          <div class="addtoCart" v-if="visible13" > 
            <div class="text"><router-link to="/cart">add to cart <span>N150</span> </router-link></div>
          </div>
          <p>Lorem</p>
        </div>
        <div class="selct2" v-on:mouseover="hoverOn14" v-on:mouseleave="hoverOff14">
          <img class="slct-img2" src="./assets/Dwomen2.png" alt="women selection">
          <div class="addtoCart" v-if="visible14" > 
            <div class="text"><router-link to="/cart">add to cart <span>N75</span> </router-link></div>
          </div>
          <p>Lorem</p>
        </div>
        <div class="selct3" v-on:mouseover="hoverOn15" v-on:mouseleave="hoverOff15">
          <img class="slct-img3" src="./assets/Dwomen3.png" alt="women selection">
          <div class="addtoCart" v-if="visible15" > 
           <div class="text"><router-link to="/cart">add to cart <span>N25</span> </router-link></div>
          </div>
          <p>Lorem</p>
        </div>
      </div>

    <div class="footer">
      <img class="footer-img" src="./assets/vueLogo.png" >
      <h2>team targaryen</h2>
    </div>
      
    </div>
</template>

<script>
import {EventBus} from '../src/main'
export default {
  components: {},
  data:  function() {
    return {
     visible1: false,
     visible2: false,
     visible3: false,
     visible4: false,
     visible5: false,
     visible6: false,
     visible7: false,
     visible8: false,
     visible9: false,
     visible10: false,
     visible11: false,
     visible12: false,
     visible13: false,
     visible14: false,
     visible15: false,
    }
  },


  methods: {
    hoverOn1: function(){
      this.visible1 = true
    },
    hoverOff1: function(){
      this.visible1 = false
    },


    hoverOn2: function(){
      this.visible2 = true
    },
    hoverOff2: function(){
      this.visible2 = false
    },
    hoverOn3: function(){
      this.visible3 = true
    },
    hoverOff3: function(){
      this.visible3 = false
    },
    hoverOn4: function(){
      this.visible4 = true
    },
    hoverOff4: function(){
      this.visible4 = false
    },
    hoverOn5: function(){
      this.visible5 = true
    },
    hoverOff5: function(){
      this.visible5 = false
    },
    hoverOn6: function(){
      this.visible6 = true
    },
    hoverOff6: function(){
      this.visible6 = false
    },


    hoverOn7: function(){
      this.visible7 = true
    },
    hoverOff7: function(){
      this.visible7 = false
    },


    hoverOn8: function(){
      this.visible8 = true
    },
    hoverOff8: function(){
      this.visible8 = false
    },


    hoverOn9: function(){
      this.visible9 = true
    },
    hoverOff9: function(){
      this.visible9 = false
    },


    hoverOn10: function(){
      this.visible10 = true
    },
    hoverOff10: function(){
      this.visible10 = false
    },


    hoverOn11: function(){
      this.visible11 = true
    },
    hoverOff11: function(){
      this.visible11 = false
    },


    hoverOn12: function(){
      this.visible12 = true
    },
    hoverOff12: function(){
      this.visible12 = false
    },



    hoverOn13: function(){
      this.visible13 = true
    },
    hoverOff13: function(){
      this.visible13 = false
    },


    hoverOn14: function(){
      this.visible14 = true
    },
    hoverOff14: function(){
      this.visible14 = false
    },


    hoverOn15: function(){
      this.visible15 = true
    },
    hoverOff15: function(){
      this.visible15 = false
    }
  }

  
}
</script>

<style scoped>




@media screen and (min-device-width: 1075px) {
  
*{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}
  
.main{
    display: block;
    width: 100%;
    height: 100%;
}

.header{
  width:90%;
  margin:0 auto;
  height: 10vh;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.header h1{
  font-size: 20px;
}
.header img{
  width: 30px;
  height: 30px;
  cursor: pointer;
}

.main .title{
  width: 90%;
  margin: 0 auto;
  margin-top: 20px;
  text-transform: uppercase;
}

.sneakers{
  width:90%;
  margin:0 auto;
  display:grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 20px;
  padding: 20px 0;
}


.jackets{
   width:90%;
  margin:0 auto;
  display:grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 20px;
  padding: 20px 0;
}
.hats{
   width:90%;
  margin:0 auto;
  display:grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 20px;
  padding: 20px 0;
}

.men{
  width:90%;
  margin:0 auto;
  display:grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 20px;
  padding: 20px 0;
}

.women{
  width:90%;
  margin:0 auto;
  display:grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 20px;
  padding: 20px 0;
}

.selct1{
  filter: drop-shadow(20px 20px 100px rgba(17, 1, 23, 0.1));
  backdrop-filter: blur(50px);
  border-radius: 10px;
}

.selct2{
  filter: drop-shadow(20px 20px 100px rgba(17, 1, 23, 0.1));
  backdrop-filter: blur(50px);
  border-radius: 10px;
}

.selct3{
  filter: drop-shadow(20px 20px 100px rgba(17, 1, 23, 0.1));
  backdrop-filter: blur(50px);
  border-radius: 10px;
}

.slct-img1{
  width: 100%;
  height: 100%;
}

.slct-img2{
  width: 100%;
  height: 100%;
}

.slct-img3{
  width: 100%;
  height: 100%;
}


.addtoCart{
 display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 10px;
  position: absolute;
  width: 50%;
  height: 12%;
  left: 25%;
  top: 83%;
  background: rgba(0, 0, 0, 0.8);
  border-radius: 5px;
  transition:all 2s ease;
}

.text{
  position: static;
  font-family: Arial;
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 28px;
  letter-spacing: 0.2em;
  color: #FFFFFF;
  flex: none;
  order: 0;
  flex-grow: 0;
  margin: 0px 10px;
  cursor:pointer;
}

.text a{
  text-decoration: none;
  color: #fff;
}

.footer{
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content:center;
  gap: 30px;
  padding-top: 20px;
}

.footer img{
  width: 50px;
  height: 50px;
}
.footer h2{
  font-size: 30px;
  text-transform: uppercase;
}


}
@media (max-width:500px){
  .sneakers{ 
    grid-template-columns: 1fr;
    gap: 60px;
  }
  .jackets{
    grid-template-columns: 1fr;
    gap: 60px;
  }
  .hats{
    grid-template-columns: 1fr;
    gap: 60px;
  }

  .men{
    grid-template-columns: 1fr;
    gap: 60px;
  }

  .women{
    grid-template-columns: 1fr;
    gap: 60px;
  }
}



</style>
