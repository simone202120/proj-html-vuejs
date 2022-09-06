<template>
    <div class="container">
        <div class="project flex">
            <div class="barra"></div>
            <p>PROJECT</p>
        </div>
        <div class="title">
            <h1>OUR EXPERT TRUSTED CONSULTANTS HELO CLIENTS</h1>
        </div>
        <div class="flex space projects">
            <SingleProject v-for="(project, index) in projects" :key="index" :Projects='project'/>
        </div>
    </div>
</template>

<script>
import SingleProject from "./SingleProject.vue";
export default {
    name:'MyProjects',

    components:{
    SingleProject
},

    data(){
        return{
            projects:[
                        {
                            imgProject:'project1',
                            descrizione:'Purinky Products',
                        },
                        {
                            imgProject:'Project2',
                            descrizione:'Purinky Products',
                        },
                        {
                            imgProject:'project3',
                            descrizione:'Purinky Products',
                        }

                    ]
        }
    }

}
</script>

<style lang="scss" scoped>

@import '../style/var.scss';
    .barra{
        width: 30px;
        border-bottom:  2px solid $Mygreen;
        margin-right: 15px;
        margin-bottom: 3px;
        height: 3px;
    }
    .project{
        align-items: flex-end;
        color:white;
        flex-wrap: wrap;
        margin-top: 50px;
        
    }
    .title{
        color: white;
        width: 50%;
        margin-top: 20px;
        line-height: 0.9;
    }
    
</style>