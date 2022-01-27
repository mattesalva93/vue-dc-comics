<template>
  <footer>
    <div class="head-footer">
      <div class="container">
        <div>
          <dc-link-card />
        </div>
        <div>
          <dc-link-card />
        </div>
        <div>
          <dc-link-card />
        </div>
        <div>
          <dc-link-card />
        </div>
        <div>
          <dc-link-card />
        </div>
      </div>
    </div>
    <div class="main-footer">
      <div class="container">
        <div class="footer-links">
          <h4>DC COMICS</h4>
          <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>Tv</li>
            <li>Games</li>
            <li>Videos</li>
            <li>News</li>
          </ul>
          <h4>SHOP</h4>
          <ul>
            <li>Shop DC</li>
            <li>Shop DC Collectibles</li>
          </ul>
          <h4>DC</h4>
          <ul>
            <li>Terms of Use</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>Tv</li>
            <li>Games</li>
            <li>Videos</li>
            <li>News</li>
            <li>Movies</li>
            <li>Tv</li>
            <li>Games</li>
            <li>Videos</li>
            <li>News</li>
          </ul>
          <h4>SITES</h4>
          <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>Tv</li>
            <li>Games</li>
          </ul>
        </div>
        <div class="container-logo">
          <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>

      </div>
    </div>
    <div class="low-footer">
      <div class="container">
        <a href="#" class="button-sign-up">
          <h4>SIGN-UP NOW!</h4>
        </a>
        <div class="icone-social">
          <h2>FOLLOW US</h2>
          <img src="../assets/img/footer-facebook.png" alt="">
          <img src="../assets/img/footer-twitter.png" alt="">
          <img src="../assets/img/footer-youtube.png" alt="">
          <img src="../assets/img/footer-periscope.png" alt="">
          <img src="../assets/img/footer-pinterest.png" alt="">
          
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
import dcLinkCard from './sub-components/dc-link-card.vue'
export default {
  components: { 
    dcLinkCard 
  },

  name:'Footer'
}
</script>

<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';
  
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

  .main-footer{
    width: 100%;
    height: 350px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    overflow-y: hidden;
    .container{
      display: flex;
      position: relative;
        .footer-links{
          width: 50%;
        }
        .container-logo{
          width: 50%;
          position: absolute;
          right: 0;
          top: -110px;
        }
    } 
  }

  .low-footer{
    width: 100%;
    height: 150px;
    background-color: #303030;
    .container{
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
      .button-sign-up{
        padding: 1px 15px;
        padding: 10px 20px;
        border: 2px solid $dcBlu;
        color:white;
        text-decoration: none;
      }
      .icone-social{
        display: flex;
        align-items: center;
        h2{
          margin-right: 20px;
          color: $dcBlu;
        }
        img{
          margin: 0 10px;
        }
      } 
    }
  }
</style>