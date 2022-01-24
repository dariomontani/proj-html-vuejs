<template>
  <div class="cards">
      <img class="first" src="..\assets\img\h3-img-1.jpg" alt="">
      <img class="center" src="..\assets\img\h3-img-2.jpg" alt="">
      <img class="center" src="..\assets\img\h3-img-3.jpg" alt="">
      <img class="last" src="..\assets\img\h3-img-4.jpg" alt="">
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
        img{
            width: calc(100% / 4);
        }
        .first{
            padding-top: 0.3em;
            padding-bottom: 0.3em;
            padding-right: 0.3em;
        }
        .center{
            padding: 0.3em;
        }
        .last{
            padding-top: 0.3em;
            padding-bottom: 0.3em;
            padding-left: 0.3em;
        }
    }
</style>