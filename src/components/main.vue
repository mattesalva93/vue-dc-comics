<template>
  <main>

      <div class="top-jumbo">

      </div>

      <div class="low-main">
          <a href="#" class="button-sign-up">
            <h4>CURRENT SERIES</h4>
          </a>
          <div class="container comics-boxes">
            <dc-comic-book
            v-for="(element, index) in comicsArray" 
            :key="index"
            :dccomic=element />
          </div>
          <div>
            <a href="#" class="button-load-more">LOAD MORE</a>
          </div>
        
      </div>

  </main>
</template>

<script>
import dcComicBook from './sub-components/dc-comic-book.vue'
export default {
  components: { dcComicBook },
  name:"Main",
  data(){
    return{
     comicsArray: [
  {
    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
    price: "$19.99",
    series: "Action Comics",
    type: "comic book"
  },
  {
    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
    price: "$3.99",
    series: "American Vampire 1976",
    type: "comic book"
  },
  {
    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
    price: "$16.99",
    series: "Aquaman",
    type: "graphic novel"
  },
  {
    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
    price: "$2.99",
    series: "Batgirl",
    type: "comic book"
  },
  {
    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    price: "$3.99",
    series: "Batman",
    type: "comic book"
  },
  {
    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    price: "$2.99",
    series: "Batman Beyond",
    type: "comic book"
  },
  {
    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
    price: "$3.99",
    series: "Batman/Superman",
    type: "comic book"
  },
  {
    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
    price: "$4.99",
    series: "Batman/Superman Annual",
    type: "comic book"
  },
  {
    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
    price: "$5.99",
    series: "Batman: The Joker War Zone",
    type: "comic book"
  },
  {
    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
    price: "$6.99",
    series: "Batman: Three Jokers",
    type: "comic book"
  },
  {
    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
    price: "$4.99",
    series: "Batman: White Knight Presents: Harley Quinn",
    type: "comic book"
  },
  {
    thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
    price: "$16.99",
    series: "Catwoman",
    type: "graphic novel"
  }
    ]
    }
  }

}
</script>

<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';

  main{
    width: 100%;
    height: 1100px;
    background-color: #1C1C1C;
    margin-top: 2px;
    .top-jumbo{
      width: 100%;
      height: 30%;
      background-image: url(../assets/img/jumbotron.jpg);
      background-repeat: no-repeat;
      background-size: cover;
    }
    .low-main{
      height: 70%;
      position:relative;
      .button-sign-up{
        padding: 12px 24px;
        border: 2px solid $dcBlu;
        background-color: $dcBlu;
        color:white;
        text-decoration: none;
        position: absolute;
        top: -20px;
        left: 25%;
      }
      .comics-boxes{
        margin: 0 auto;
        width: 80%;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;

      }
      div{
        margin: 35px 0;
        text-align: center;
        .button-load-more{
  
          padding: 12px 24px;
          border: 2px solid $dcBlu;
          background-color: $dcBlu;
          color:white;
          text-decoration: none;
        }
      }

    }
  }

</style>