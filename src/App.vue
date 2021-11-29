<template>

    <div>
   <app-shop class="app"></app-shop>

    <div class="data">
      <h1>{{msg}}</h1>
       <h2>{{love}}</h2>
    </div>

   </div>
   
    
    
 
</template>

<script>
import Shop from './Shop'

export default {
  components: {
    'app-shop': Shop,
  },

  data:  function() {
    return {
      msg: 'The page is currently on production, only avaliable on mobile and desktop  . please switch to the right device to view',
      love: 'with love from dev team'
    }
  }
}
</script>

<style scoped>

*{
  margin: 0;
  padding: 0;
  font-family: Arial, Helvetica, sans-serif;
}



@media screen and (min-device-width: 1075px)   {

.app{display: block;}
.data{display: none;}

}

@media screen and (max-device-width: 1024px)   {

.app{display: none;}
.data{display: block;}

h1{
  position: absolute;
  top: 30%;
  width:96%;
  left:2%;
  line-height: 60px;
  letter-spacing: 10px;
  text-align: center;
  color: black;
  font-size: 25px;
  font-family: 'Courier New', Courier, monospace;
  text-transform: capitalize;
  margin: 30px auto;
}

h2{
  position: absolute;
  top: 80%;
  width:96%;
  left:2%;
  line-height: 60px;
  letter-spacing: 10px;
  text-align: center;
  color:grey;
  font-size: 15px;
  font-family: 'Courier New', Courier, monospace;
  text-transform:uppercase;
}

}

@media screen and (max-device-width: 480px)  {
    .app{display: block;}
    .data{display: none;}

}




</style>
