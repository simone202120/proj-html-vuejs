<template>
  <div class="article">
    <p>{{Article.articolo}}</p>
    <h3>{{Article.autore}}</h3>
    <p>{{Article.publisher}}</p>
  </div>
</template>

<script>
export default {
    name:'SingleArticle',

    props:{
        Article:Object
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/general.scss';
    @import '../style/var.scss';

    .article{
        width: 30%;
        padding: 30px;

        P{
            color:$SmallText;
            font-size: 14px;
        }

        h3{
            color:$BlueText;
            margin-top: 30px;
            margin-bottom: 10px;
        }
    }

</style>