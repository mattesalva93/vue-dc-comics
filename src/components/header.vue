<template>
  <header>
    <div class="container">
      <div>
        <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <div>
        <ul>
          <li v-for="(link, indice) in navlinks" :key="indice" :class="{'active': link.current}">
              <a :href="link.url" >{{link.text}}</a>
          </li>
        </ul>
      </div>
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
        line-height: 125px;
        &.active, &:hover {
          color: $dcBlu;
          border-bottom: 3px solid $dcBlu;
        }
        a{
          text-decoration: none;
          text-transform: uppercase;

        }
      }
  }



</style>