<template>
    <div class="jumbo">
        <button class="prev"><strong>PREV</strong></button>
        <div class="container">
            <div class="urban"><img src="..\assets\img\h3-rev-img-5.png" alt=""></div>
            <div class="pizza"><img src="..\assets\img\h3-rev-img-6.png" alt=""></div>
        </div>
        <button class="next"><strong>NEXT</strong></button>
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
        background: linear-gradient(90deg, black (100px - 1px), transparent 1%) center, linear-gradient(black (100px - 1px), transparent 1%) center,#EBEBDE;
	    background-size: 100px 100px; 
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