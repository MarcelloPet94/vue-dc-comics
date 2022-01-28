<template>
  <div>
    <div class="main">
      <imgBackground/>
      <div class="thumb_container">
        <Thumb v-for="(item , indice) in prodotto" :key="indice"
        :img="item.thumb"
        :category="item.series"
        />
      </div>  
    </div>
  </div>
</template>

<script>
import imgBackground from './Component/ImgBackground.vue'
import Thumb from './Component/Thumb.vue'
import infoprod from '../data/dc-comics.js'

export default {
  name: 'Main',
  components:{
    imgBackground,
    Thumb
  },
  data(){
    return{
      prodotto : infoprod
    }
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
  }
}  
</style>
