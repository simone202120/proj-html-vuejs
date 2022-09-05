<template>
  <main>
    <div class="flex sectionTitle">
        <h3>OUR CONSULTANTS CAN HELP YOU</h3>
        <div class="bar"></div>
    </div>
    <div class="container flex wrap space">
        <ServiceCard v-for="(service, index) in services" :key="index" :card="service"/>
    </div>
  </main>
</template>

<script>
    import ServiceCard from './ServiceCard.vue';
export default {
    name:'MyService',
    components: {
        ServiceCard
    },

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
    
</style>