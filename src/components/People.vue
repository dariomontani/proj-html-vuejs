<template>
    <div class="people">
        <div class="container">
            <div class="containerHover">
                <h2>FRANK BAILEY</h2>
                <p class="arial">Kitchen Porter</p>
                <div>
                    <i class="fab fa-instagram-square" style="margin: 0.5em;"></i><i class="fab fa-twitter" style="margin: 0.5em;"></i><i class="fab fa-facebook-f" style="margin: 0.5em;"></i>
                </div>
            </div>
            <img src="..\assets\img\h1-team-1a-700x700.jpg" alt="">
        </div>
        <div class="container">
            <div class="containerHover">
                <h2>FRANK BAILEY</h2>
                <p class="arial">Kitchen Porter</p>
                <div>
                    <i class="fab fa-instagram-square" style="margin: 0.5em;"></i><i class="fab fa-twitter" style="margin: 0.5em;"></i><i class="fab fa-facebook-f" style="margin: 0.5em;"></i>
                </div>
            </div>
            <img src="..\assets\img\h1-team-2a.jpg" alt="">
        </div>
        <div class="container">
            <div class="containerHover">
                <h2>FRANK BAILEY</h2>
                <p class="arial">Kitchen Porter</p>
                <div>
                    <i class="fab fa-instagram-square" style="margin: 0.5em;"></i><i class="fab fa-twitter" style="margin: 0.5em;"></i><i class="fab fa-facebook-f" style="margin: 0.5em;"></i>
                </div>
            </div>
            <img src="..\assets\img\h1-team-3a.jpg" alt="">
        </div>
        <div class="container">
            <div class="containerHover">
                <h2>FRANK BAILEY</h2>
                <p class="arial">Kitchen Porter</p>
                <div>
                    <i class="fab fa-instagram-square" style="margin: 0.5em;"></i><i class="fab fa-twitter" style="margin: 0.5em;"></i><i class="fab fa-facebook-f" style="margin: 0.5em;"></i>
                </div>
            </div>
            <img src="..\assets\img\h1-team-4a.jpg" alt="">
        </div>
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
        .container{
            position: relative;
            width: calc(100% / 4);
            cursor: pointer;
            img{
                width: 100%;
            }
            .containerHover{
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
                display: flex;
                flex-direction: column;
                align-items: center;
                justify-content: center;
                background-color: #EE2852;
                border: 20px solid white;
                color: white;
                width: 100%;
                height: 100%;
                line-height: 2em;
                display: none;
                .arial{
                    font-family: Arial, Helvetica, sans-serif;
                    font-size: 0.8em;
                }
            }
        }
        .container:hover .containerHover{
            display: flex;
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