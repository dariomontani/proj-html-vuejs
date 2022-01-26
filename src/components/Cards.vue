<template>
    <div class="cards">
        <div class="container first">
            <div class="eye">
            <i class="fas fa-eye" style="font-size: 2em; z-index: 999; color: white;"></i>
            </div>
            <img src="..\assets\img\h3-img-1.jpg" alt="">
            <div class="background"></div>
        </div>
        <div class="container center">
            <div class="eye">
            <i class="fas fa-eye" style="font-size: 2em; z-index: 999; color: white;"></i>
            </div>
            <img src="..\assets\img\h3-img-2.jpg" alt="">
            <div class="background"></div>
        </div>
        <div class="container center">
            <div class="eye">
            <i class="fas fa-eye" style="font-size: 2em; z-index: 999; color: white;"></i>
            </div>
            <img src="..\assets\img\h3-img-3.jpg" alt="">
            <div class="background"></div>
        </div>
        <div class="container last">
            <div class="eye">
            <i class="fas fa-eye" style="font-size: 2em; z-index: 999; color: white;"></i>
            </div>
            <img src="..\assets\img\h3-img-4.jpg" alt="">
            <div class="background"></div>
        </div>
    </div>
</template>

<script>
export default {
    name:"Cards"
}
</script>

<style lang="scss">
    .cards{
        display: flex;
        justify-content: space-between;
        .container{
            width: calc(100% / 4);
            position: relative;
            .eye{
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
                background-color: #EE2852;
                padding: 2em;
                border-radius: 50%;
                z-index: 99;
                font-size: 0.8em;
                display: none;
                cursor: pointer;
            }
            img{
                width: 100%;
            }
            .background{
                border: 1px solid black;
                position: absolute;
                top: 0;
                width: 349px;
                height: 240px;
                background: linear-gradient(90deg, black (8px - 1px), transparent 1%) center, linear-gradient(black (8px - 1px), transparent 1%) center,#EBEBDE;
                filter: invert(1);
                background-size: 8px 8px;
                display: none;
                
            }
        }
        .first{
            margin-top: 0.3em;
            margin-bottom: 0.3em;
            margin-right: 0.3em;
        }
        .center{
            margin: 0.3em;
        }
        .last{
            margin-top: 0.3em;
            margin-bottom: 0.3em;
            margin-left: 0.3em;
        }
        .container:hover .background{
            display: block;
        }
        .container:hover .eye{
            display: block;
        }
    }
</style>