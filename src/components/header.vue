<template>
  <header>
    <div class="container">
      <div>
        <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <nav>
        <ul>
          <li v-for="(link, indice) in navlinks" :key="indice">
              <a :href="link.url" :class="{'active': link.current}">{{link.text}}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name:'Header',
  data() {
    return {
      navlinks: [

        {
            text: "Characters",
            url: "#",
            current: false,
        },
        {
            text: "Comics",
            url: "#",
            current: true,
        },
        {
            text: "Movies",
            url: "#",
            current: false,
        },
        {
            text: "Tv",
            url: "#",
            current: false,
        },
        {
            text: "Games",
            url: "#",
            current: false,
        },
        {
            text: "Collectibles",
            url: "#",
            current: false,
        },
        {
            text: "Videos",
            url: "#",
            current: false,
        },
        {
            text: "Fans",
            url: "#",
            current: false,
        },
        {
            text: "News",
            url: "#",
            current: false,
        },
        {
            text: "Shop",
            url: "#",
            current: false,
        }
        
      ]

    }
  }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';

  .container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 125px;
      li{
        display: inline-block;
        margin: 0 10px;
        a{
          text-decoration: none;
          text-transform: uppercase;
          line-height: 125px;
          color: $coloreTesto;
          &.active, &:hover {
            color: $dcBlu;
            padding: 51px 0;
            border-bottom: 5px solid $dcBlu;
          }
        }
      }
  }



</style>