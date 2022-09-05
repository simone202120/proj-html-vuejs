<template>
    <div class="serviceCard flex">
        <div class="icon"><i :class=card.icon></i></div>
        <div class="description">
            <h2>{{card.service}}</h2>
            <p>{{card.description}}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ServiceCard',

    props:{
        card:Object
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/var.scss';
    
     .serviceCard{
        width:40%;
        margin: 30px;
    }
    .icon{
        background-color:#f81e3a;
        height: 50px;
        width: 50px;
        border-radius: 50%;
        margin-right: 20px;
        display: flex;
        justify-content: center;
        align-items: center;
        color: white;
        
    }
    .description{
        width: 80%;

        h2{
            margin-bottom: 20px;
            color:$BlueText;
        }
    }
</style>