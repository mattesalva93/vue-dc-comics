<template>
      <div class="main-footer">
      <div class="container">
        <div class="footer-links">
          <div>
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
            <h4>DC COMICS</h4>
            <ul>
              <li>Characters</li>
              <li>Comics</li>
            </ul>
          </div>

          <div>
            <h4>DC COMICS</h4>
            <ul>
              <li>Characters</li>
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
          </div>

          <div>
            <h4>DC COMICS</h4>
            <ul>
              <li>Characters</li>
              <li>Comics</li>
              <li>Movies</li>
            </ul>
          </div>
        </div>

        <div class="container-logo">
          <img src="../../assets/img/dc-logo-bg.png" alt="">
        </div>

      </div>
    </div>
</template>

<script>
export default {
    name: 'Footer-main',

}
</script>

<style lang="scss" scoped>
@import '../../assets/style/partials/variables.scss';

  .main-footer{
    width: 100%;
    height: 350px;
    background-image: url(../../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    overflow-y: hidden;
    .container{
      position: relative;
        .footer-links{
          display: flex;
          width: 50%;
          div{
          margin-right: 20px;
          }
          h4{
            margin-top: 30px;
            color: white;
          }
          ul{
            list-style-type: none;
            margin: 15px 0;
            color: grey;
            font-size: 0.9rem;
          }
        }
        .container-logo{
          width: 50%;
          position: absolute;
          right: 0;
          top: -110px;
        }
    } 
  }
</style>