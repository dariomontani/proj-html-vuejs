<template>
  <div class="cit">
      <img src="..\assets\img\h3-testimonials-bckgrnd.jpg" alt="">
      <div class="top"><h2>"</h2></div>
      <div class="center"><h2>"FORGET THE TRENDY PIZZA SHOPS, THIS HIDDEN SPOT MAKES THE BEST NEW YORK-STYLE PIZZA SLICE IN NAPLES"</h2></div>
      <div class="bottom"><p>WASHINGTON POST 2018</p></div>
  </div>
</template>

<script>
export default {
    name:"Cit"
}
</script>

<style lang="scss">
    .cit{
        width: 100%;
        height: 400px;
        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
        div{
            text-align: center;
        }
        .center{
            width: 54%;
        }
        .bottom{
            padding-top: 1em;
            color: #D2401E;
            font-size: 0.8em;
        }
        img{
            position: absolute;
            max-width: 100%;
            z-index: -1;
        }
    }
</style>