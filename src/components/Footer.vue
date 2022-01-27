<template>
  <div class="main_footer">
    <Strip/>
    <div class="footer_info">
        <div class="info_box">
            <ul>
            <li>lista</li>
            <li>lista</li>
            <li>lista</li>
            </ul>  
            <ul>
            <li>lista</li>
            <li>lista</li>
            <li>lista</li>
            </ul>  
        </div>
        <div class="info_box">
            <ul>
            <li>lista</li>
            <li>lista</li>
            <li>lista</li>
            </ul>  
        </div>   
        <div class="info_box">
            <ul>
            <li>lista</li>
            <li>lista</li>
            <li>lista</li>
            </ul>  
        </div>    
    </div>
  </div>
</template>

<script>

import Strip from  './Strip.vue'

export default {
  name: 'Footer',
  components: {
    Strip
  }
}
</script>

<style scoped lang="scss">

/* IMPORT > VARIABLES */
@import '../assets/partials/variables.scss';

.main_footer
{
  background-color: blue;
  background-image: url(../assets/img/footer-bg.jpg);


    .footer_info
    {
        display: flex;
        margin: 0 auto;
        width: $mainWidth;
        background-image: url(../assets/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-size: 40%;
        background-position: center right;


        ul li:first-of-type
        {
            font-weight: 800;
            line-height: 48px;
        }
        ul li
        {
            color: $darkMode;
        };
    }

    .info_box
    {
        padding: 24px 24px 24px 0;
    }
}

</style>
