<template>
    <div class="container">
        <div class="flex space box">
            <div class="logoSmall">
                <img src="../assets/logosmall.png" alt="">
            </div>
            <div class="nav">
                <ul class="flex">
                    <li v-for="(voice, index) in menu" :key="index">
                        <a href="">{{voice}}</a>
                    </li>
                </ul>
            </div>
            <div class="social">
                <i class="fa-brands fa-instagram"></i>
                <i class="fa-brands fa-linkedin-in"></i>
                <i class="fa-brands fa-facebook-f"></i>
                <i class="fa-brands fa-twitter"></i>
            </div>
        </div>
        <div class="flex space terms">
            <p>Terms of use <br> Privacy Enviromental Policy</p>
            <p>Copyrigt 2020 bla bla bla bla bla Reserved</p>
        </div>
    </div>
</template>

<script>
export default {
    name:'FootBar',

    props:{
        menu:Array
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/general.scss';
    @import '../style/var.scss';

    .container{
        padding-top:50px;

        .box{
            padding-bottom: 50px;
            border-bottom: 2px solid rgba($color: #9796a2, $alpha: 0.1);
        }
    }

    .logoSmall{
        img{
            width: 100px;
        }
    }
    a{
        color:$SmallText;
        padding: 0 10px 0 10px;
        font-size: 14px;
    }
    .social i{
        color: white;
        padding: 0 10px 0 10px;
    }
    .terms{
        color: $SmallText;
        padding:20px 0 20px 0;
        font-size: 12px;
    }

</style>