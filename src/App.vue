<template>
  <div id="app">
    <MyJumbotron @copia="caricaMenu" />
    <MyService />
    <AboutUs/>
    <MyProjects/>
    <MyTestimonials/>
    <MyBlog/>
    <MyFooter :menu="menu"/>
  </div>
</template>

<script>
import MyJumbotron from './components/MyJumbotron.vue';
import MyService from './components/MyService.vue';
import AboutUs from './components/AboutUs.vue';
import MyProjects from './components/MyProjects.vue';
import MyTestimonials from './components/MyTestimonials.vue';
import MyBlog from './components/MyBlog.vue';
import MyFooter from './components/MyFooter.vue';


export default {
  name: 'App',
  components: {
    MyJumbotron,
    MyService,
    AboutUs,
    MyProjects,
    MyTestimonials,
    MyBlog,
    MyFooter
},

  data(){
    return{
      menu:""
    }
  },
  methods:{
    caricaMenu(vociMenu){
      this.menu=vociMenu;
      return this.menu
    }
  }
}
</script>

<style lang="scss">
  @import './style/general.scss';
  @import './style/var.scss';
  @import '~@fortawesome/fontawesome-free/css/all.css'

</style>
