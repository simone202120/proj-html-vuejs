<template>
  <div class="background ">
        <div class="container flex spaceBetween">
            <div class="logo">
                <img id="logo" src="../assets/logotype.png" alt="">
            </div>
            
            <div class="nav">
                <ul class="flex">
                    <li v-for="(voice, index) in MenuVoices" :key="index">
                        <a href="">{{voice}}</a>
                    </li>
                </ul>
            </div>
        </div>

        <div class="title">
            <div class="flex">
                <div class="barra"></div>
                    <p>ALWAIS THE BEST WAY YOU NEED IT</p>
                </div>
                <H1>THE BEST BUSINESS CONSULTING</H1>
                <div class="buttons flex">
                    <button><a href="#"></a>READ MORE</button>
                <div class="play flex">
                    <a href=""><i class="fa-solid fa-play"></i></a>
                </div>
            </div>
        </div>
  </div>
</template>

<script>
export default {
    name:'MyHeader',

    data(){
        return{
            MenuVoices:['HOME', 'ABOUT', 'PROJECTS', 'SERVICES', 'BLOG','CONTACT']
        }
    },

    methods:{
        copiaMenu(){
        return this.$emit('copia',this.MenuVoices)
        }
    },

    mounted(){
        this.copiaMenu()
    }
}

</script>

<style lang="scss" scoped>
     @import '../style/var.scss';
   .background{
    background-image: url('../assets/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg');
    background-size: 60%;
    background-repeat: no-repeat;
    background-position-x: right;
    padding-bottom: 50px;
   
   }
   .spaceBetween{
    justify-content: space-between;
   }

   li{
    padding: 20px 5px;
        &:hover{
            border-top: solid 2px white;
            font-weight: bolder;
        }
   }
   #logo{
    height: 20px;
   }
   .logo{
    padding: 20px;
    height: 40px;
   }
   .nav{
    height: 30px;
   }
   .title{
    color: white;
    width: 40%;
    margin-left: 11%;
    margin-top: 100px;
   }
   .barra{
    width: 30px;
    border-bottom:  2px solid $Mygreen;
    margin-right: 15px;
    margin-bottom: 3px;
   }
   button{
    background-color: $Mygreen;
    width: 150px;
    transition-duration: 1s;

        &:hover{
            scale: 1.2;
            background-color: $MyRed;
            color: white;
        }
   }
   .play{
        width: 40px;
        height: 40px;
        border: 2px solid white;
        border-radius: 50%;
        margin-left: 20px;
        justify-content: center;
        align-items: center;
        transition-duration: 1s;

        a{
            color: $Mygreen;
        }

        &:hover{
            scale: 1.2;
        }
   }

   h1{
        font-size: 95px;
        margin:20px 0 40px 0;
        line-height: 0.8;
   }
   
</style>
