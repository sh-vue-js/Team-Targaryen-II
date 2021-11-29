<template>

    <div class="cart">
         <div class="header">
            <router-link to="/"><h1>Shopping Website.</h1></router-link>
            <img src="./assets/cartCheck.png">
        </div>
        <div class="main">
          
          <div class="title">
            <p>Product</p>
            <p>Description</p>
            <p>Quantity</p>
            <p>Price</p>
            <p>Remove</p>
          </div>
          <hr id="un">
          <div class="product product1">
            <img src="./assets/Dsneaks1.png" alt="sneakers selection">
            <p id="desc">Lorem</p>
            <p id="quantity"><input type="number" v-model="product1" @change="calculateTotal"></p>
            <p id="price">N25</p>
            <p id="remove" @click="removeProduct1">x</p>
          </div>

          <div class="product product2">
            <img src="./assets/Dwomen2.png" alt="sneakers selection">
            <p id="desc">Lorem</p>
            <p id="quantity"><input type="number" v-model="product2" @change="calculateTotal"></p>
            <p id="price">N75</p>
            <p id="remove" @click="removeProduct2">x</p>
          </div>
          <hr>
        <p id="total">Total: N{{totalprice}}</p>
        </div>
      </div>
    

</template>

<script>
export default {
  data(){
    return{
      totalprice: 100,
      product1: 1,
      product2: 1,
    }
  },
  methods:{
    calculateTotal(){
      let sumofProduct1 = this.product1 * 25
      let sumofProduct2 = this.product2 * 75
      let sum = sumofProduct1 + sumofProduct2
      this.totalprice = sum
    },
    removeProduct1(){
      document.querySelector('.product1').style.display = 'none'
      this.product1 = 0
      this.calculateTotal()
    },
    removeProduct2(){
      document.querySelector('.product2').style.display = 'none'
      this.product2 = 0
      this.calculateTotal()
    }
  }
}
</script>

<style scoped>
*{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
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
.header a{
    text-decoration: none;
    color: black;
}
.header img{
  width: 30px;
  height: 30px;
  cursor: pointer;
}



.cart .main{
  width: 80%;
  margin: 0 auto;
  padding: 20px 0;
}

.cart .main .title{
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  place-content: center;
  padding-bottom:10px;
}

.cart .main .title p{
  width: 100%;
}

.cart .main #total{
  text-align: right;
  padding-top: 20px;
  font-size: 50px;
}

.cart .main .product{
  padding: 20px 0;
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  place-items: center;
}

.cart .main .product #quantity{
  width: 100%;
}

.cart .main .product #quantity input{
  width: 50%;
  margin: 0 auto;
  padding: 10px;
  border: 1px solid green;
  outline: none;
  text-align: center;
  font-size: 15px;
}

.cart .main .product #remove{
  font-weight: bolder;
  cursor: pointer;
}

.cart .main .product p{
  width: 100%;
}

.cart .main .product img{
  width: 100%;
  height: 200px;
}

@media (max-width:950px){
  .cart .main .title{
    display: none;
  }
  #un{
    display: none;
  }
  .cart .main .product{
    gap: 20px;
  }
  .cart .main .product img{
    width: 100%;
    height: 100px;
  }
}

@media (max-width:500px){
  .cart .main .product img{
      width: 100%;
      height: 60px;
  }
  .cart .main .product #quantity input{
    width: 100%;
    margin: 0 auto;
    padding: 10px;
    border: 1px solid green;
    outline: none;
    text-align: center;
    font-size: 13px;
  }
  .cart .main #total{
    font-size: 25px;
  }
}
</style>