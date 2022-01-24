<template>
    <div class="navbar">
        <div class="left">
            <button><h4>ORDER ONLINE</h4></button>
        </div>
        <div class="center">
            <div class="home"><img src="..\assets\img\svg-0.svg" alt=""><span>HOME</span></div> 
            <div>PAGES</div>
            <div>MENU</div>
            <img class="logo" src="..\assets\img\h5-logo-divided-header.png" alt="">
            <div>EVENT</div>
            <div>BLOG</div>
            <div>LANDING</div>
        </div>
        <div class="right">
            <div class="cart"><img src="..\assets\img\svg-1.svg" alt="">CART</div>
            <div class="search">SEARCH</div>
        </div>
    </div>
</template>

<script>
export default {
    name:"Navbar"
}
</script>

<style lang="scss" scope>
    .navbar{
        background-color: black;
        color: white;
        padding-top: 1em;
        display: flex;
        justify-content: space-around;
        align-items: center;
        .left{
            button{
                background-color: #EE2852;
                border: #EE2852;
                color: #FFFFFF;
                padding: 1em;
            }
        }
        .center{
            display: flex;
            justify-content: space-between;
            align-items: center;
            .home{
                display: flex;
                padding-right: 2em;
                img{
                    filter: invert(1);
                }
            }
            .logo{
                width: 30%;
                background-color: black;
            }
        }
        .right{
            display: flex;
            .cart img{
                filter: invert(1);
            }
            div{
                padding: 0 1em;
            }
        }
    }
</style>