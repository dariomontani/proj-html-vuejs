<template>
    <div class="tipeOfPizza">
        <div v-for="(pizza, index) in pizzas" :key="index" class="pizza">
            <img class="zoom" :src="`${pizza.img}`" alt="">
            <p class="namePizza">{{pizza.type}}</p>
            <p class="price">{{pizza.price}}</p>
        </div>
        <!-- <div class="pizza">
            <img src="" alt="">
            <p class="namePizza"></p>
            <p class="price"></p>
        </div>
        <div class="pizza">
            <img src="" alt="">
            <p class="namePizza"></p>
            <p class="price"></p>
        </div>
        <div class="pizza">
            <img src="" alt="">
            <p class="namePizza"></p>
            <p class="price"></p>
        </div>
        <div class="pizza">
            <img src="" alt="">
            <p class="namePizza"></p>
            <p class="price"></p>
        </div>
        <div class="pizza">
            <img class="zoom" src="" alt="">
            <p class="namePizza"></p>
            <p class="price"></p>
        </div> -->
    </div>
</template>

<script>
export default {
    name:"TipeOfPizza",
    data(){
      return {
        pizzas: [
          {
            img: require('../assets/img/h3-product-img-1a-100x100.png'),
            type: "BISMARK",
            price: "$5.00 - $30.00",
          },
          {
            img: require('../assets/img/h3-product-img-2a-150x150.png'),
            type: "FIORI DI ZUCCA",
            price: "$7.00 - $50.00",
          },
          {
            img: require('../assets/img/h3-product-img-3a-150x150.png'),
            type: "VALDOSTANA",
            price: "$55.00",
          },
          {
            img: require('../assets/img/h3-product-img-4a-150x150.png'),
            type: "PIZZA TARTUFATA",
            price: "$45.00",
          },
          {
            img: require('../assets/img/h3-product-img-5a-150x150.png'),
            type: "FRANCESCANA",
            price: "$25.00",
          },
          {
            img: require('../assets/img/h3-product-img-6a-100x100.png'),
            type: "CAMPAGNOLA",
            price: "$50.00 - $95.00",
          },
        ],
      }
    }
}
</script>

<style lang="scss">
    .tipeOfPizza{
        padding-top: 2em;
        padding-bottom: 5em;
        display: flex;
        justify-content: space-around;
        .pizza{
            text-align: center;
            perspective: 100px;
            cursor: pointer;
            .zoom{
                width: 9.4em;
            }
            .namePizza{
                color: #B7903C;
                font-size: 0.8em;
                padding-top: 1em;
            }
            .price{
                color: #D2401E;
                font-size: 0.8em;
            }
        }
        .pizza:hover img{
            transform: translateZ(20px);
        }
    }
</style>