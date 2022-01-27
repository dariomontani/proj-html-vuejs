<template>
    <div class="delishPizza">
        <div class="left">

            <div class="title">
                <div>
                    <p class="red">MADE WITH LOVE</p>
                    <h1 class="white">DELISH PIZZA DEALS</h1>
                </div>
            </div>

            <div v-for="(deal, index) in deals" :key="index" class="deal">
                <div class="date">
                    <h1 class="red">{{deal.day}}</h1>
                    <h3 class="white">{{deal.month}}</h3>
                </div>
                <div class="text">
                    <h3 class="white">{{deal.title}}</h3>
                    <p class="red location">{{deal.address}}</p>
                </div>
            </div>

            <!-- <hr> -->

            <!-- <div class="deal">
                <div class="date">
                    <h1 class="red">03</h1>
                    <h3 class="white">NOV</h3>
                </div>
                <div class="text">
                    <h3 class="white"></h3>
                    <p class="red location">204 E. Pizzetta Tommaso</p>
                </div>
            </div>

            <hr>

            <div class="deal">
                <div class="date">
                    <h1 class="red">05</h1>
                    <h3 class="white">NOV</h3>
                </div>
                <div class="text">
                    <h3 class="white"></h3>
                    <p class="red location"></p>
                </div>
            </div> -->
        </div>
        <div class="right">
            <img src="..\assets\img\h3-img-5a.jpg" alt="">
        </div>
    </div>
</template>

<script>
export default {
    name:"DelishPizza",
    data(){
        return{
            deals: [
                {
                    day:"02",
                    month:"NOV",
                    title:"TRADITIONAL NEOPOLITAN PIES IN KYOTO PIZZA MERCATO",
                    address:"204 E. Pizzetta Tommaso",
                },
                {
                    day:"03",
                    month:"NOV",
                    title:"TERARAZZA PATIO DINING SPACE OPENING THIS WEEKEND",
                    address:"204 E. Pizzetta Tommaso",
                },
                {
                    day:"05",
                    month:"NOV",
                    title:"SIENNA PRIVATE DINING ROOM WITH STÉPHANE BRUNN",
                    address:"204 E. Pizzetta Tommaso",
                },
            ],
        }
    }
}
</script>

<style lang="scss">
    .delishPizza{
        display: flex;
        .left{
            border: 1px solid white;   
            height: 550px;
            width: calc(100% / 2);
            background: linear-gradient(90deg, black (100px - 1px), transparent 1%) center, linear-gradient(black (100px - 1px), transparent 1%) center,#EBEBDE;
	        background-size: 100px 100px; 
            display: flex;
            flex-direction: column;
            align-items: center;
            padding-top: 2em;
            .title{
                width: 60%;
            }
            .deal{
                display: flex;
                justify-content: center;
                width: 60%;
                padding: 2em 0;
                .location{
                    font-size: 0.8em;
                }
                .date{
                    padding-right: 2em;
                }
            }
            hr{
                border: 1px dotted #B7903C;
                width: 60%;
            }
            .red{
                color: #D2401E;
            }
            .white{
                color: white;
            }
        }
        .right{
            width: calc(100% / 2);
            img{
                width: 100%;
            }
        }
    }
</style>