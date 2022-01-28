<template>
  <div class="box_thumb">
          <div class="img_thumb">
            <img :src="img" alt="">
          </div>
      <p>{{category}}</p>
  </div>                                            
</template>

<script>

export default {
  name: 'Main',
  props: {
      img: String,
      category: String
  }
}
</script>

<style scoped lang="scss">
/* IMPORT > VARIABLES */
@import '../../assets/partials/variables.scss';

.box_thumb
{
  margin: 16px 0 16px;
  width: calc(10vw - 1vw);

}

.img_thumb
{
  height: calc(10vw - 1vw);
  overflow: hidden;    

    img
    {
      width: 100%;
  }
}

.box_thumb p 
{
  font-size: 0.9em;
  margin-top: 16px;
  color: #fff;
  text-transform: uppercase;
}

</style>
