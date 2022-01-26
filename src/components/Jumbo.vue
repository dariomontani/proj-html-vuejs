<template>
    <div class="jumbo">
        <div class="urban"><img src="..\assets\img\h3-rev-img-5.png" alt=""></div>
        <button @click="prev" type="button" class="prev">PREV</button>
        <div class="container">
            <div class="pizza">
                <img src="../assets/img/h3-rev-img-6.png" alt="">
                <!-- <img :src="`${images[n]}`" alt=""> -->
            </div>
        </div>
        <button @click="next" type="button" class="next">NEXT</button>
    </div>
</template>

<script>

export default {
    name:"Jumbo",
    data: function(){
        return{
            n: 0,
            images: [
                '../assets/img/h3-rev-img-2.png',
                '../assets/img/h3-rev-img-4.png',
                '../assets/img/h3-rev-img-6.png',
                // 'https://picsum.photos/id/237/200/300',
            ],
        }
    },
    methods: {
        next: function(){
            this.n += 1
            if(this.n == this.images.length){
                this.n = 0;
            }
        },
        prev: function(){
            this.n -= 1
            if(this.n < 0){
                this.n = this.images.length - 1;
            }
        },
    },
}
</script>

<style lang="scss" scope>
    .jumbo{
        height: 550px;
        background: linear-gradient(90deg, black (100px - 1px), transparent 1%) center, linear-gradient(black (100px - 1px), transparent 1%) center,#EBEBDE;
	    background-size: 100px 100px;
        .urban{
                position: absolute;
                left: 50%;
                top: 50%;
                transform: translate(-50%, -50%);
        }
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
            cursor: pointer;
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
            cursor: pointer;
        }
        .container{
            position: relative;
            padding-top: 5em;
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