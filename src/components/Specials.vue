<template>
    <div class="specials">
        <div class="left">
            <img class="background" src="..\assets\img\h1-img-4.jpg" alt="">
            <img class="logoSpecials" src="..\assets\img\h1-img-7n.png" alt="">
        </div>
        <div class="right">
            <ul>
                <li>
                    <h2>SPECIALS*</h2>
                    <p class="arialn">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Praesent ut.</p>
                </li>
                <li>
                    <h3><span class="red">$10</span>COMBO PICCOLO</h3>
                    <ul>
                        <li>
                            <p class="arial">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Praesent ut aliquam dui.</p>
                        </li>
                    </ul>
                </li>
                <li>
                    <h3><span class="red">$20</span>COMBO MEZZO</h3>
                    <ul>
                        <li>
                            <p class="arial">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Praesent ut aliquam dui.</p>
                        </li>
                    </ul>
                </li>
                <li>
                    <h3><span class="red">$30</span>COMBO GRANDE</h3>
                    <ul>
                        <li>
                            <p class="arial">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Praesent ut aliquam dui.</p>
                        </li>
                    </ul>
                </li>
            </ul>
            <div class="pizzaLogo">
                <ul>
                    <li>
                        <img src="..\assets\img\svg-4.svg" alt="">
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:"Specials"
}
</script>

<style lang="scss">
    .specials{
        display: flex;
        .left{
            width: calc(100% / 2);
            position: relative;
            .background{
                width: 100%;
            }
            .logoSpecials{
                width: 40%;
                position: absolute;
                left: 50%;
                top: 50%;
                transform: translate(-50%, -50%);
            }
        }
        .right{
            width: calc(100% / 2);
            padding: 0 8em;
            line-height: 2.5em;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            ul{
                list-style: none;
            }
            .arialn{
                font-family: Arial, Helvetica, sans-serif;
                color: #B2B2B2;
                line-height: 1.5em;
            }
            .arial{
                font-family: Arial, Helvetica, sans-serif;
                color: #B2B2B2;
                line-height: 1.5em;
                margin-left: 3em;
            }
            .red{
                color: #D2401E;
                padding-right: 1em;
            }
            .pizzaLogo{
                width: 155%;
                text-align: right;
                ul li img{
                    background-color: #F7F7F2;
                    padding: 1em;
                    border-radius: 50%;
                }
            }
        }
    }

</style>