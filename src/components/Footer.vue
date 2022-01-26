<template>
  <footer>
    <div class="left">
      <div class="up">
        <div class="find">
          <h3 class="brown">FIND OUR RESTAURANTS</h3>
          <ul>
            <li v-for="(restaurant, index) in restaurants" :key="index" class="arial gray">
              {{restaurant.adress}}
              <!-- 1614 E.Bell Rd #104. <br>
              Salerno, AZ 85022 <br>
              &lpar;602&rpar; 867-1010 -->
            </li>

            <!-- <li class="arial gray">
              204 E.Pizzetta Tommaso <br>
              Salerno, AZ 85022 <br>
              &lpar;358&rpar; 867-1010
            </li>

            <li class="arial gray">
              Valle Puglia 54 <br>
              Torre Del Greco AZ 85022 <br>
              &lpar;359&rpar; 867-1010
            </li>

            <li class="arial gray">
              Corso Itali AA <br>
              Naples, AZ 85022 <br>
              &lpar;989&rpar; 867-1010
            </li> -->
          </ul>
        </div>

        <div class="working">
          <h3 class="brown">WORKING HOURS</h3>
          <ul>
            <li>
              <h5 class="brown">MONDAY</h5>
              <p class="arial red">Kitchen Closed</p>
            </li>
            <li>
              <h5 class="brown">TUSEDAY UNTIL FRIDAY</h5>
              <p class="arial gray">9:00 - 22:00</p>
            </li>
            <li>
              <h5 class="brown">SATURDAY <span class="red">*</span></h5>
              <p class="arial gray">Saturday 11am to midnight</p>
            </li>
            <li>
              <h5 class="brown">SUNDAY</h5>
              <p class="arial gray">9:00 - 22:00</p>
            </li>
            <li>
              <h5 class="brown">FOLLOW US</h5>
            </li>
          </ul>
        </div>
        <div class="bigText">
          <h2 class="white">THE DON PEPPE CREW <br>
          FIRST AND FOREMOST <br>
          VALUE AN AUTHENTIC, <br>
          WELL BAKED SLICE OF <br>
          PIZZA.</h2>
        </div>
      </div>
      <div class="down arial">
        <p class="brown">Created with &#x2661; by <span class="green">Qode Interactive</span></p>
      </div>
    </div>
    <div class="right">
      <img src="..\assets\img\footer-img-1.jpg" alt="">
    </div>
  </footer>
</template>

<script>
export default {
    name: "Footer",
    data(){
      return {
        restaurants: [
          {
            adress: "1614 E.Bell Rd #104. Salerno, AZ 85022  (602)867-1010"
          },
          {
            adress: "204 E.Pizzetta Tommaso Salerno, AZ 85022 (358)867-1010"
          },
          {
            adress: "Valle Puglia 54 Torre Del Greco AZ 85022 (359)867-1010"
          },
          {
            adress: "Corso Itali AA Naples, AZ 85022 (989)867-1010"
          }
        ],
      }
    }
}
</script>

<style lang="scss" scope>
  footer{
    display: flex;
    ul{
      list-style: none;
      li{
        padding-top: 1em;
        line-height: 1.6em;
      }
    }
    .left{
      width: calc(100% /2);
      background: linear-gradient(90deg, black (100px - 1px), transparent 1%) center, linear-gradient(black (100px - 1px), transparent 1%) center,#EBEBDE;
	    background-size: 100px 100px; 
      color: white;
      display: flex;
      flex-direction: column;
      justify-content: center;
      .brown{
        color: #B7903C;
      }
      .gray{
        color: #B2B2B2;
      }
      .red{
        color: #D2401E;
      }
      .green{
        color: #339966;
      }
      .arial{
        font-family: Arial, Helvetica, sans-serif;
      }
      .up{
        display: flex;
        justify-content: center;
        .working{
          padding: 0 2em;
        }
        .find{
          width: 25%;
        }
      }
      .down{
        padding-top: 3em;
        padding-left: 2.5em;
        font-size: 0.8em;
      }
    }
    .right{
      width: calc(100% / 2);
      img{
        width: 100%;
      }
    }
  }
</style>