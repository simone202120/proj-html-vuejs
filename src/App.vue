<template>
  <div id="app">
    <MyJumbotron />
    <MyService />
  </div>
</template>

<script>
import MyJumbotron from './components/MyJumbotron.vue';
import MyService from './components/MyService.vue';

export default {
  name: 'App',
  components: {
    MyJumbotron,
    MyService
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
