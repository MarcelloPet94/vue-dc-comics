<template>
  <div>
    <div class="main">
      <imgBackground/>
      <div class="thumb_container">
        <div class="label">
          <span>current series</span>
        </div>
        <div class="box_thumb">
          <div class="img_thumb">
            <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8" alt="">
          </div>
          <p>Titolo</p>
        </div>                                            
      </div>
    </div>
  </div>
</template>

<script>
import imgBackground from './Component/ImgBackground.vue'

export default {
  name: 'Main',
  components:{
    imgBackground
  }
}
</script>

<style scoped lang="scss">
/* IMPORT > VARIABLES */
@import '../assets/partials/variables.scss';

.main
{
  background-color: #010101;

  .thumb_container
  {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    position: relative;
    width: 60vw;
    margin: 0 auto;

    .box_thumb
    {
      margin: 16px 0 16px;
      width: calc(10vw - 1vw);


      .img_thumb
      {
        height: calc(10vw - 1vw);
        overflow: hidden;    

          img
          {
            width: 100%;
        }
      }
    }  

    .box_thumb p 
    {
      font-size: 0.9em;
      margin-top: 16px;
      color: #fff;
      text-transform: uppercase;
    }

    .label 
    {
      position: absolute;
      top: -3.5em;
      left: -0.5em;
      background-color: blue;

      span
      {
        font-size: 2em;
        color: #fff;
        padding: 0 16px;
        line-height: 1.5em;
      }
    }  
  }
}  
</style>
