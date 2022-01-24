<template>
  <div class="specials">
      <div class="left">
          <img class="background" src="..\assets\img\h1-img-4.jpg" alt="">
          <img class="logoSpecials" src="..\assets\img\h1-img-7n.png" alt="">
      </div>
      <div class="right">
          <ul>
              <li>asfdasdfsf</li>
              <li>asfdasdfsf</li>
              <li>asfdasdfsf</li>
              <li>asfdasdfsf</li>
              <li>asfdasdfsf</li>
          </ul>
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
    }

</style>