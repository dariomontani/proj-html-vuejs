<template>
    <div class="tipeOfPizza">
        <div class="pizza">
            <img class="zoom" src="..\assets\img\h3-product-img-1a-100x100.png" alt="">
            <p class="namePizza">BISMARK</p>
            <p class="price">$5.00 - $30.00</p>
        </div>
        <div class="pizza">
            <img src="..\assets\img\h3-product-img-2a-150x150.png" alt="">
            <p class="namePizza">FIORI DI ZUCCA</p>
            <p class="price">$7.00 - $50.00</p>
        </div>
        <div class="pizza">
            <img src="..\assets\img\h3-product-img-3a-150x150.png" alt="">
            <p class="namePizza">VALDOSTANA</p>
            <p class="price">$55.00</p>
        </div>
        <div class="pizza">
            <img src="..\assets\img\h3-product-img-4a-150x150.png" alt="">
            <p class="namePizza">PIZZA TARTUFATA</p>
            <p class="price">$45.00</p>
        </div>
        <div class="pizza">
            <img src="..\assets\img\h3-product-img-5a-150x150.png" alt="">
            <p class="namePizza">FRANCESCANA</p>
            <p class="price">$25.00</p>
        </div>
        <div class="pizza">
            <img class="zoom" src="..\assets\img\h3-product-img-6a-100x100.png" alt="">
            <p class="namePizza">CAMPAGNOLA</p>
            <p class="price">$50.00 - $95.00</p>
        </div>
    </div>
</template>

<script>
export default {
    name:"TipeOfPizza"
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