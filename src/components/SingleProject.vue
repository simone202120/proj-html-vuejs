<template>
  <div class="project">
    <div class="hover flex">
       <h3>{{Projects.descrizione}}</h3>
       <p class="categoria">{{Projects.categoria}}</p>
    </div>
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
     @import '../style/var.scss';
    .project{
        width:32%;
        margin-bottom: 70px;

        img{
            width: 100%;
        }
        &:hover{
            .hover{
                display: inline-block;
            }
        }
    }
    .hover{
        height: 243px;
        width: 324px;
        display: none;
        background-color:rgba($color: #e20b0b, $alpha: 0.6);
        position: absolute;
        padding: 20px;

        h3{
            margin-top:150px
        }
    }
    .categoria{
        color:$SmallText;
    }
</style>