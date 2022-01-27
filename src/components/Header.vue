<template>
  <section class="header">
    <div class="align_content_header">
      <div class="logo_img">
          <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <nav class="right_navigation">
        <ul>
          <li class="nav_menu">
            <a href="#">voce</a>
          </li>
          <li class="nav_menu">
            <a href="#">voce</a>
          </li>
          <li class="nav_menu">
            <a href="#">voce</a>
          </li>
          <li class="nav_menu">
            <a href="#">voce</a>
          </li>
          <li class="nav_menu">
            <a href="#">voce</a>
          </li>
        </ul>
      </nav>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Header',
}
</script>

<style scoped lang="scss">
/* GLOBAL STYLE */
@import '../assets/partials/style.scss';
/* IMPORT > VARIABLES */
@import '../assets/partials/variables.scss';

  .header
  {
    background-color: lightgrey;

    .align_content_header
    {
      display: flex;
      justify-content: space-between;
      margin: 0 auto;
      width: 80%;
      background-color: #fff;
      border: 1px solid red;
        
        .logo_img
        {
          width: 90px;
          padding: 8px;

          img
          {
            width: 100%;
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
            list-style-type: none;
            padding: 0 8px;
            border: 1px solid #010101;

            a
            {
              text-decoration: none;
              color: $baseColor;
              padding: 0 24px;
              border: 1px solid #010101;
            }
          }
        }
      }
    }  
  }

</style>
