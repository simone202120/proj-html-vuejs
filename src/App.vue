<template>
  <div id="app">
    <MyJumbotron />
  </div>
</template>

<script>
import MyJumbotron from './components/MyJumbotron.vue';


export default {
  name: 'App',
  components: {
    MyJumbotron
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
