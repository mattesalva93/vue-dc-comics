<template>
    <div class="head-footer">
      <div class="container">
        <dc-link-card 
        v-for="(element,index) in dclinks"
        :key="index"
        :dclink="element" />

      </div>
    </div>
</template>

<script>
import dcLinkCard from './dc-link-card.vue'
export default {

    components: { 
        dcLinkCard 
        },
    name: 'Footer-head',
    data (){
      return {
        dclinks: [
            {
            src: require("../../assets/img/buy-comics-digital-comics.png"),
            title: 'DIGITAL COMICS',
            },
            {
            src: require("../../assets/img/buy-comics-merchandise.png"),
            title: 'DC MERCHANDISE',
            },
            {
            src: require("../../assets/img/buy-comics-shop-locator.png"),
            title: 'SUBSCRIPTIONS',
            },
            {
            src: require("../../assets/img/buy-comics-subscriptions.png"),
            title: 'COMIC SHOP LOCATOR',
            },
            {
            src: require("../../assets/img/buy-dc-power-visa.svg"),
            title: 'DC POWER VISA',
            },
        ]
      }
    }

}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

  .head-footer{
    width: 100%;
    background-color: $dcBlu;
    height: 165px;
    z-index: 12;
    .container{
      display: flex;
      justify-content: space-around;
    }
  }
</style>