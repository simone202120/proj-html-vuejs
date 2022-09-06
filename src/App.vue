<template>
  <div id="app">
    <MyJumbotron />
    <MyService />
    <AboutUs/>
    <MyProjects/>
    <MyTestimonials/>
    <MyBlog/>
    <MyFooter/>
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

    }
  }
}
</script>

<style lang="scss">
  @import './style/general.scss';
  @import './style/var.scss';
  @import '~@fortawesome/fontawesome-free/css/all.css'

</style>
