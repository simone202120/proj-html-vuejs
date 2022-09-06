<template>
<main>
    <div class="testimonials container">
        <div class="title flex">
            <p>TESTIMONIALS</p>
            <div class="barra"></div>
        </div>
        <div class="titolo">
            <h1>WHAT'S THE COUSTOMER SAY ABOUT OUR WORK</h1>
        </div>
    </div>
    <div class="boxArticle flex">
        <SingleArticle v-for="(Article, index) in Articles" :key="index" :Article="Article" />
    </div>
</main>
</template>

<script>
import SingleArticle from './SingleArticle.vue';
export default {
    name: "MyTestimonials",
    data() {
        return {
            Articles: [
                {
                    articolo: "When, while lovely valley teems with vapour around meand  eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknow plants are noticed by when i hear the buzz of the little.",
                    autore: "Vera Duncan",
                    publisher: "Amazon Inc"
                },
                {
                    articolo: "When, while lovely valley teems with vapour around meand  eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknow plants are noticed by when i hear the buzz of the little.",
                    autore: "Vera Duncan",
                    publisher: "Amazon Inc"
                },
                {
                    articolo: "When, while lovely valley teems with vapour around meand  eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknow plants are noticed by when i hear the buzz of the little.",
                    autore: "Vera Duncan",
                    publisher: "Amazon Inc"
                }
            ]
        };
    },
    components: { SingleArticle }
}
</script>

<style lang="scss" scoped>
    @import '../style/var.scss';
    @import '../style/general.scss';
    
    .barra{
        width: 30px;
        border-bottom:  2px solid $Mygreen;
        margin-right: 15px;
        margin-bottom: 3px;
        height: 3px;
        margin-left: 20px;
    }
    .title{
        color: white;
        align-items: flex-end;
        margin-bottom: 20px;
        justify-content: flex-end;
        
    }
    .titolo{
        color: white;
        line-height: 0.9;
        text-align: end;
        display: block;
    }
    .testimonials{
        width: 30%;
        margin-right: 10%;
    }
    .boxArticle{
        background-color: white;
        margin-top: 50px;
        width: 90%;
        margin-left: 10%;
   }
    
    
</style>