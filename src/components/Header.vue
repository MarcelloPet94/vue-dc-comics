<template>
  <section class="header">
    <div class="align_content_header">
      <div class="logo_img">
          <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <nav class="right_navigation">
        <ul>
          <li class="nav_menu" :class="{selected : elementi.current}" v-for="(elementi , indice) in links" :key="indice">
            <a href="#" :class="{textSelected : elementi.current}">{{elementi.text}}</a>
          </li>
        </ul>
      </nav>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Header',
   data() {
      return{
        links: [
            {
                text: "Home",
                url: "#",
                current: false,
            },
            {
                text: "Prodotti",
                url: "#",
                current: true,
            },
            {
                text: "Chi Siamo",
                url: "#",
                current: false,
            },
            {
                text: "Contatti",
                url: "#",
                current: false,
            },
        ]
      }
    }
}
</script>

<style scoped lang="scss">
/* IMPORT > VARIABLES */
@import '../assets/partials/variables.scss';

  .header
  {
    .align_content_header
    {
      display: flex;
      justify-content: space-between;
      margin: 0 auto;
      width: $mainWidth;
      background-color: #fff;
        
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
            padding: 0 8px;

            a
            {
              color: $baseColor;
              padding: 0 24px;
            }
            a.textSelected
            {
              color: blue;
            }
          }
        }
      }
      .selected
      {
            border-bottom: 4px solid blue;
      }
    }  
  }

</style>
