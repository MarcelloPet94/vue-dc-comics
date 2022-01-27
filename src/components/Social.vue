<template>
  <section class="social">
    <div class="align_content_header">
      <div class="logo_img">
          <a href="#">shop up now</a>
      </div>
      <nav class="right_navigation">
        <ul>
          <li class="nav_menu">
            <a href="#">
              follow us
            </a>
          </li>
          <li class="nav_menu">
            <a href="#">
              <img src="../assets/img/footer-facebook.png" alt="">

            </a>
          </li>
          <li class="nav_menu">
            <a href="#">
              <img src="../assets/img/footer-twitter.png" alt="">

            </a>
          </li>
          <li class="nav_menu">
            <a href="#">
              <img src="../assets/img/footer-youtube.png" alt="">

            </a>
          </li>
          <li class="nav_menu">
            <a href="#">
              <img src="../assets/img/footer-pinterest.png" alt="">

            </a>
          </li>
          <li class="nav_menu">
            <a href="#">
              <img src="../assets/img/footer-periscope.png" alt="">

            </a>
          </li>
        </ul>
      </nav>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Social',
}
</script>

<style scoped lang="scss">
/* IMPORT > VARIABLES */
@import '../assets/partials/variables.scss';

  .social
  {
    background-color: #333;
    
    .align_content_header
    {
      display: flex;
      justify-content: space-between;
      margin: 0 auto;
      width: $mainWidth;
        
        .logo_img
        {
          display: flex;
          align-items: center;

          a
          {
            color: $darkMode;
            padding: 8px 16px;
            border: 4px solid blue;
          }
        }


      .right_navigation
      {
        display: flex;
        align-items: center;

        ul
        {
          display: flex;
          height: 90px;

          li
          {
            display: flex;
            align-items: center;
            padding: 0 8px;

            a
            {
              color: $darkMode;
            }
          }
        }
      }
    }  
  }

</style>
