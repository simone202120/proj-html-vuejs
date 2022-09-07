<template>
    <footer>
        <div class="containerfoot">
            <div class="box flex">
                <h1>LET'S TALK ABOUT WORK</h1>
                <div class="testofoot">
                    <p>A wonderful serenity has taken possession Far far away, behind the word mountains</p>
                </div>
                <button><a href="#">GET STARTED</a></button>
            </div>
        </div>
        <FootBar :menu="menu"/>
    </footer>
</template>

<script>
import FootBar from './FootBar.vue';
export default {
    name: "MyFooter",
    props: {
        menu: Array
    },
    components: { FootBar }
}
</script>

<style lang="scss" scoped>
    @import '../style/general.scss';
    @import '../style/var.scss';

.containerfoot{
    margin-top: 200px;
    background-image: url('../assets/foot.jpg');
    background-size: 100% 100%;
    padding: 80px;
    color: white;
    justify-content: center;
    align-items: center;
    text-align: center;
}

.testofoot{
    width: 300px;
    text-align: center;

    p{
        margin-bottom: 20px;
        margin-top: 10px;
    }
}
.box{
    flex-direction:column;
    align-items: center;
}
button{
    background-color: $BlueText;
    width: 150px;
    height: 40px;
    transition-duration: 1s;
    &:hover{
        scale: 1.1;
        background-color: $Mygreen;

        a{
            color:$BlueText;
        }
        
    }
}


</style>