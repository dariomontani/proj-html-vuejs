<template>
    <div class="buildPizza">
        <img src="..\assets\img\h3-background-img.jpg" alt="">
        <div class="text">
            <h1>GO AHEAD AND BUILD YOUR OWN PIZZA <br> WE WON'T JUDGE!</h1>
        </div>
     </div>
</template>

<script>
export default {
    name:"BuildPizza"
}
</script>

<style lang="scss">
    .buildPizza{
        position: relative;
        img{
            width: 100%;
            height: 450px;
            object-fit: cover;
        }
        .text{
            width: 15%;
            color: white;
            position: absolute;
            top: 25%;
            left: 25%;
        }
    }
</style>