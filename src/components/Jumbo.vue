<template>
    <div class="jumbo">
        <div class="container">
            <div class="urban"><img src="..\assets\img\h3-rev-img-5.png" alt=""></div>
            <div class="pizza"><img src="..\assets\img\h3-rev-img-6.png" alt=""></div>
        </div>
    </div>
</template>

<script>

export default {
    name:"Jumbo"
}
</script>

<style lang="scss" scope>
    .jumbo{
        height: 550px;
        background-color: black;
        .container{
            position: relative;
            padding-top: 5em;
            .urban{
                position: absolute;
                left: 50%;
                top: 50%;
                transform: translate(-50%, 0%);
            }
            .pizza{
                position: absolute;
                position: absolute;
                left: 50%;
                top: 50%;
                transform: translate(-50%, 0%);
            }
        }
    }
</style>