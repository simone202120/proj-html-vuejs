<template>
  <div id="app">
    <MyJumbotron />
    <MyService />
    <AboutUs/>
    <MyProjects/>
  </div>
</template>

<script>
import MyJumbotron from './components/MyJumbotron.vue';
import MyService from './components/MyService.vue';
import AboutUs from './components/AboutUs.vue';
import MyProjects from './components/MyProjects.vue';

export default {
  name: 'App',
  components: {
    MyJumbotron,
    MyService,
    AboutUs,
    MyProjects
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
