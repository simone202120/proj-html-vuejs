<template>
  <div class="CardArticle">
    <img :src="require('../assets/'+ Articolo.img + '.jpg')" alt="">
    <div class="CorpoArticolo">
        <p class="data-autore">{{Articolo.data}} {{Articolo.autore}}</p>
        <h2>{{Articolo.titolo}}</h2>
        <p class="corpo">{{Articolo.corpo}}</p>
    </div>
  </div>
</template>

<script>
export default {
    name:'BlogArticle',

    props:{
        Articolo:Object
    }
}
</script>

<style lang="scss" scoped>
@import '../style/general.scss';
@import '../style/var.scss';

    .CardArticle{
       width: 49%;
       margin-top:40px;
       position: relative;
    }
    img{
        width: 100%;
    }
    .CorpoArticolo{
        padding: 30px;
        width: 80%;
        background-color: white;
        position: absolute;
        right: 0;
        top:60%;
    }
    .corpo{
        color:$SmallText;
        margin-top:20px;
    }
    .data-autore{
        color:$MyRed;
        margin-bottom: 20px;
        font-weight: bold;
    }
    .prova{
        height: 300px;
    }
</style>