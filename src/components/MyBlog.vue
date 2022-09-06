<template>
  <div class="container">
    <div class="flex intestazione">
        <div class="barra"></div>
        <p>BLOG</p>
    </div>
    <div class="flex space title">
        <h1>THE RECENT NEWS YOU MUST READ IT</h1>
        <button><a href="#">VIEW ALL</a></button>
    </div>
    <div class="BlogContainer flex space">
        <BlogArticle v-for="(articolo, index) in Articoli" :key="index" :Articolo="articolo"/>
    </div>
  </div>
</template>

<script>
import BlogArticle from './BlogArticle.vue';
export default {
    name: "MyBlog",
    components: { BlogArticle },

    data(){
        return{
            Articoli:[
                        {
                            titolo:'Canadian Consulting Firm acquired by UK Giant',
                            data:'july 4,2019',
                            autore:'by Paul',
                            corpo:'When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a...',
                            img:'blog1'
                        },
                        {
                            titolo:'Canadian Consulting Firm acquired by UK Giant',
                            data:'july 4,2019',
                            autore:'by Paul',
                            corpo:'When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a...',
                            img:'blog2'
                        }
                    ]
        }
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/general.scss';
    @import '../style/var.scss';

    .barra{
        width: 30px;
        border-bottom:  2px solid $Mygreen;
        margin-right: 15px;
        margin-bottom: 3px;
        height: 3px;
    }
    .intestazione{
        color:white;
        align-items: flex-end;
        margin-top:100px;
    }
    .title{
        margin-top:30px;
        h1{
            color:white;
        }
        button{
        background-color:$Mygreen;
        width: 150px;
            a{
                color:$BlueText; 
                font-weight: bold;
            }

        }
    }
   

    
    
</style>