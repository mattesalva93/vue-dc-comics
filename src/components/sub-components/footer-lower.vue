<template>
    <div class="low-footer">
      <div class="container">
        <a href="#" class="button-sign-up">
          <h4>SIGN-UP NOW!</h4>
        </a>
        <div class="icone-social">
          <h2>FOLLOW US</h2>
          <img src="../../assets/img/footer-facebook.png" alt="">
          <img src="../../assets/img/footer-twitter.png" alt="">
          <img src="../../assets/img/footer-youtube.png" alt="">
          <img src="../../assets/img/footer-periscope.png" alt="">
          <img src="../../assets/img/footer-pinterest.png" alt="">
        </div>
      </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

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