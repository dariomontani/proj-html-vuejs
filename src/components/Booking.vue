<template>
    <div class="booking">
        <img class="background" src="..\assets\img\h3-background-img-3.jpg" alt="">
        <div class="whiteSpace"><p>1 Person</p><p><i class="fas fa-user-friends"></i></p></div>
        <div class="forAt"><p>FOR</p></div>
        <div class="whiteSpace"><p>11/29/2020</p><p><i class="fas fa-calendar"></i></p></div>
        <div class="forAt"><p>AT</p></div>
        <div class="whiteSpace"><p>7:00 pm</p><p><i class="fas fa-clock"></i></p></div>
        <div class="button">
            <button>BOOK A TABLE</button>
        </div>
    </div>
</template>

<script>
export default {
    name:"Booking"
}
</script>

<style lang="scss">
    .booking{
        height: 220px;
        position: relative;
        display: flex;
        justify-content: center;
        align-items: center;
        .background{
            position: absolute;
            width: 100%;
            z-index: -1;
        }
        .whiteSpace{
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 0.5em;
            border: 1px solid black;
            background-color: white;
            height: 60px;
            width: 200px;
            font-family: Arial, Helvetica, sans-serif;
            color: #B7903C;
        }
        .forAt{
            padding: 0 3em;
            color: white;
        }
        .button{
            padding-left: 5em;
            button{
                color: white;
                background-color: #EE2852;
                border: #EE2852;
                padding: 1.5em 4em;
            }
        }
    }
</style>