<template>

<router-view/>

</template>

<script>
import home from '../components/home'


export default {
    data:  function() {
        return {
         switchCom: 'app-sneakers'
        }
    },
    components: {
        'home': home,  
    }
}
</script>

<style scoped >

*{box-sizing: border-box; 
    margin: 0 ;
    padding: 0;
}

   .main{position: relative;
         height: 100vh;
         width: 100vw;
         padding: 0;
         margin: 0;
         background: white;   }

    

/*all media queries are applied to mobile devices et tablet */

@media screen and  (min-device-width: 1075px)  {

.component-switch{display: none;}

}

@media screen and  (max-device-width: 1024px)  {

.component-switch{display: none;}

}
   
@media screen and  (max-device-width: 480px)  {
  


   .component-switch{
       display: block;
       position: absolute;
       width: 71.67vw;
       height: 5vh;
       left: 13.56vw;
       top: 24.38vh;
       overflow-x: scroll;
       z-index: 2;
   }

   .component-list{
       display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    position: absolute;
    width: 950px;
    height: 16px;
    left: 0px;
    top: 50%;
  
   }

   button{text-decoration: none;
     font-size: 40px;
     position: absolute;
     background: transparent;
   
   }

   .selection1{
       position: static;
    width: 77px;
    height: 16px;
    left: 0px;
    top: 0px;
    font-family: Arial;
    font-style: normal;
    font-weight: normal;
    font-size:35px;
    line-height: 16px;
    display: flex;
    align-items: center;
    text-align: right;
    letter-spacing: 0.2em;
    text-transform: lowercase;
    color: #141415;
    flex: none;
    order: 0;
    flex-grow: 0;
    margin: 0px 124px;

   }

   .selection2{
       position: static;
    width: 61px;
    height: 16px;
    left: 211px;
    top: 0px;
    font-family: Arial;
    font-style: normal;
    font-weight: normal;
    font-size:35px;
    line-height: 16px;
    display: flex;
    align-items: center;
    text-align: right;
    letter-spacing: 0.2em;
    text-transform: lowercase;
    color: #141415;
    flex: none;
    order: 1;
    flex-grow: 0;
    margin: 0px 104px;
   }

   .selection3{
       position: static;
    width: 26px;
    height: 16px;
    left: 206px;
    top: 0px;
    font-family: Arial;
    font-style: normal;
    font-weight: normal;
    font-size:35px;
    line-height: 16px;
    display: flex;
    align-items: center;
    text-align: right;
    letter-spacing: 0.2em;
    text-transform: lowercase;
    color: #141415;
    flex: none;
    order: 2;
    flex-grow: 0;
    margin: 0px 54px;
   }

   .selection4{
       position: static;
    width: 26px;
    height: 16px;
    left: 266px;
    top: 0px;
    font-family: Arial;
    font-style: normal;
    font-weight: normal;
    font-size:35px;
    line-height: 16px;
    display: flex;
    align-items: center;
    text-align: right;
    letter-spacing: 0.2em;
    text-transform: lowercase;
    color: #141415;
    flex: none;
    order: 3;
    flex-grow: 0;
    margin: 0px 194px;
   }

   .selection5{
       position: static;
    width: 26px;
    height: 16px;
    left: 326px;
    top: 0px;
    font-family: Arial;
    font-style: normal;
    font-weight: normal;
    font-size:35px;
    line-height: 16px;
    display: flex;
    align-items: center;
    text-align: right;
    letter-spacing: 0.2em;
    text-transform: lowercase;
    color: #141415;
    flex: none;
    order: 4;
    flex-grow: 0;
    margin: 0px 0px;
   }




  

}








</style>
