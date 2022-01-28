<template>
  <div id="test" class="icon_strip">
    <div class="align_all_icon">
        <div class="component_box">
            <img src="../assets/img/buy-comics-digital-comics.png">
            <a href="#">digital comics</a>
        </div>
        <div class="component_box">
            <img src="../assets/img/buy-comics-merchandise.png">
            <a href="#">digital comics</a>
        </div>
        <div class="component_box">
            <img src="../assets/img/buy-dc-power-visa.svg">
            <a href="#">digital comics</a>
        </div>
        <div class="component_box">
            <img src="../assets/img/buy-comics-shop-locator.png">
            <a href="#">digital comics</a>
        </div>
        <div class="component_box">
            <img src="../assets/img/buy-comics-subscriptions.png">
            <a href="#">digital comics</a>
        </div>
    </div>    
  </div>
</template>

<script>


export default {
  name: 'Strip',
}
</script>

<style scoped lang="scss">
/* IMPORT > VARIABLES */
@import '../assets/partials/variables.scss';

.icon_strip
{
  background-color: royalblue;

    .align_all_icon
    {
    display: flex;
    align-items: center;
    margin: 0 auto;
    padding: 24px 0;
    width: $mainWidth;
    }
        .component_box
        {
            display: flex;
            align-items: center;
            width: 20%;

                img
                {
                width: 56px;
                }
        }

    .component_box a
    {
    color: $darkMode;
    padding: 0 16px;
    }
}
</style>
