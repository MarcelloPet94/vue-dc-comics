<template>
  <div>
    <div class="main">
      <imgBackground/>
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
.main
{
  height: 1000px;
  background-color: #010101;

  h3
  {
    text-align: center;
    line-height: 100px;
    color: #fff;
  }
}  
</style>
