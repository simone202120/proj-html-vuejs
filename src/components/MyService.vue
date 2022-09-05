<template>
  <main>
    <div class="flex sectionTitle">
        <h3>OUR CONSULTANTS CAN HELP YOU</h3>
        <div class="bar"></div>
    </div>
    <div class="container flex wrap space">
        <div v-for="(service, index) in services" :key="index" class="serviceCard flex">
            <div class="icon"><i :class=service.icon></i></div>
            <div class="description">
                <h2>{{service.service}}</h2>
                <p>{{service.description}}</p>
            </div>
        </div>
    </div>
  </main>
</template>

<script>
export default {
    name:'MyService',

    data(){
        return{
            services:[
                {
                    service:'STATISTICAL CONSULTING',
                    description:'When while lovely valley teems with vapour around meand eridan sun strikes the upper impenetrable foliage of my trees,and but a ',
                    icon:"fa-solid fa-chart-line"
                },
                {
                    service:'DIGITAL CONSULTING',
                    description:'When while lovely valley teems with vapour around meand eridan sun strikes the upper impenetrable foliage of my trees,and but a ',
                    icon:"fa-solid fa-bullhorn"
                },
                {
                    service:'BANKING CONSULTING',
                    description:'When while lovely valley teems with vapour around meand eridan sun strikes the upper impenetrable foliage of my trees,and but a ',
                    icon:"fa-solid fa-wallet"
                },
                {
                    service:'ENTERPRISE CONSULTING',
                    description:'When while lovely valley teems with vapour around meand eridan sun strikes the upper impenetrable foliage of my trees,and but a ',
                    icon:"fa-solid fa-bullseye"
                }

            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/var.scss';
    main{
        background-color: white;
    }
    .bar{
        border-bottom:  3px solid $Mygreen;
        height: 2px;
        width: 73%;
        margin-left: 30px;
    }
    .sectionTitle{
        margin-left: 11%;
        padding-top: 70px;
        align-items: center;
        margin-bottom: 60px;
    }
    h3{
        color:$BlueText
    }

    /* Regole stile per card service */
    
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