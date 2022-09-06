<template>
  <div class="project">
   <img :src="require('../assets/'+ Projects.imgProject + '.jpg')" alt="">
  </div>
</template>

<script>
export default {
    name:'SingleProject',

    props:{
        Projects: Object
    }
}
</script>

<style lang="scss" scoped>
    .project{
        width:32%;
        margin-bottom: 70px;

        img{
            width: 100%;
        }
    }
</style>