<template>
    <div class="cit">
        <img src="..\assets\img\h3-testimonials-bckgrnd.jpg" alt="">
        <button class="prev"><strong>PREV</strong></button>
        <div class="top">
            <h2><i class="fas fa-quote-left"></i></h2>
        </div>
        <div class="center">
            <h2>"FORGET THE TRENDY PIZZA SHOPS, THIS HIDDEN SPOT MAKES THE BEST NEW YORK-STYLE PIZZA SLICE IN NAPLES"</h2>
        </div>
        <div class="bottom">
            <p>WASHINGTON POST 2018</p>
        </div>
        <button class="next"><strong>NEXT</strong></button>
        <img class="pizzaLogo" src="..\assets\img\svg-4.svg" alt="">
    </div>
</template>

<script>
export default {
    name:"Cit"
}
</script>

<style lang="scss">
    .cit{
        width: 100%;
        height: 400px;
        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
        .prev{
            transform: rotate(90deg);
            position: absolute;
            top: 50%;
            left: 0;
            border: 1px solid white;
            background-color: white;
            border-top-left-radius: 100% 200%;
            border-top-right-radius: 100% 200%;
            padding: 0.5em 1.5em;
            color: #EE2852;
        }
        .next{
            transform: rotate(270deg);
            position: absolute;
            top: 50%;
            right: 0;
            border: 1px solid white;
            background-color: white;
            border-top-left-radius: 100% 200%;
            border-top-right-radius: 100% 200%;
            padding: 0.5em 1.5em;
            color: #EE2852;
        }
        .top h2{
            font-size: 3.5em;
            color: #B7903C;
        }
        div{
            text-align: center;
        }
        .center{
            width: 54%;
        }
        .bottom{
            padding-top: 1em;
            color: #D2401E;
            font-size: 0.8em;
        }
        img{
            position: absolute;
            max-width: 100%;
            z-index: -1;
        }
        .pizzaLogo{
            position: absolute;
            right: 1em;
            bottom: 2em;
        }
    }
</style>