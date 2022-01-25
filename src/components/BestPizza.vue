<template>
    <div class="bestPizza">
        <div class="red">
            <p>CHOSE YOUR FLAVOR</p>
        </div>
        <div class="center">
            <h1>THE BEST PIZZA MENU IN TOWN</h1>
        </div>
        <div class="bottom">
            <p class="arial">Lorem ipsum dolor sit amet consectetur adipisicing elit. Beatae illo inventore ut, qui numquam nesciunt quo quidem. temporibus molestias.</p>
        </div>
        <img class="pizzaLogo" src="..\assets\img\svg-4.svg" alt="">
    </div>
</template>

<script>
export default {
    name:"Bestpizza"
}
</script>

<style lang="scss">
    .bestPizza{
        height: 300px;
        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
        div{
            text-align: center;
        }
        .center{
            padding: 0.8em 0;
        }
        .red{
            color: #D2401E;
            font-size: 0.8em;
        }
        .bottom .arial{
            font-family: Arial, Helvetica, sans-serif;
            width: 60%;
            margin: auto;
        }
        .pizzaLogo{
            position: absolute;
            right: 1em;
            bottom: 2em;
        }
    }
</style>