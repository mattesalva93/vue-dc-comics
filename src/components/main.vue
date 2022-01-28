<template>
  <main>

      <div class="top-jumbo">

      </div>

      <div class="low-main">
          <a href="#" class="button-sign-up">
            <h4>CURRENT SERIES</h4>
          </a>
        
      </div>

  </main>
</template>

<script>
export default {
  name:"Main",
}
</script>

<style lang="scss" scoped>
@import '../assets/style/partials/variables.scss';

  main{
    width: 100%;
    height: 1000px;
    background-color: #1C1C1C;
    margin-top: 2px;
    .top-jumbo{
      width: 100%;
      height: 40%;
      background-image: url(../assets/img/jumbotron.jpg);
      background-repeat: no-repeat;
      background-size: cover;
    }
    .low-main{
      height: 60%;
      position:relative;
      .button-sign-up{
        padding: 12px 24px;
        border: 2px solid $dcBlu;
        background-color: $dcBlu;
        color:white;
        text-decoration: none;
        position: absolute;
        top: -20px;
        left: 500px;
      }

    }
  }

</style>