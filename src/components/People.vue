<template>
    <div class="people">
        <img src="..\assets\img\h1-team-1a-700x700.jpg" alt="">
        <img src="..\assets\img\h1-team-2a.jpg" alt="">
        <img src="..\assets\img\h1-team-3a.jpg" alt="">
        <img src="..\assets\img\h1-team-4a.jpg" alt="">
        <img class="pizzaLogo" src="..\assets\img\svg-4.svg" alt=""> 
    </div>
</template>

<script>
export default {
    name:"People"
}
</script>

<style lang="scss">
    .people{
        position: relative; 
        display: flex;
        img{
            width: calc(100% / 4);
        }
        .pizzaLogo{
            position: absolute;
            width: 2.6em;
            background-color: #F7F7F2;
            border-radius: 50%;
            padding: 0.8em;
            right: 1em;
            bottom: 2em;
        }
    }
</style>