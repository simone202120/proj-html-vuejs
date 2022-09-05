<template>
  <div class="background">
        <div class="about flex">
            <div class="barra"></div>
            <p>ABOUT US</p>
        </div>
        <div class="description">
            <h1>WE MAKE YOUR STRATEGY WORK</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusamus velit quaerat quos repellendus qui, sit laudantium laborum nemo dignissimos aut reiciendis quasi consectetur sequi? Quisquam explicabo quos eaque a consectetur?</p>
        </div>
        <div class="CTA flex">
            <div class="flexItem">
                <h2>WE HELP TO DELIVER THE BUSINESS CASE</h2>
            </div>
            <div  class="flexItem">
                <p>When while lovely valley teems with vapour around meand eridan sun strikes the upper impenetrable foliage of my trees,and but a rhousand unknow</p>
            </div>
            
        </div>
  </div>
</template>

<script>
export default {
    name:'AbautUs'
}
</script>

<style lang="scss" scoped>
@import '../style/var.scss';
    .background{
        background-image: url('../assets/aboutUs.jpg');
        background-size: 50%;
        background-repeat: no-repeat;
        background-position-x: left;
        padding-bottom: 50px;
    }

   .barra{
        width: 30px;
        border-bottom:  2px solid $Mygreen;
        margin-right: 15px;
        margin-bottom: 3px;
    }
   .description{
        width: 30%;
        margin-left: 60%;
        padding-bottom: 100px;
    
        h1{
            font-size:50px;
            color: white;
            line-height: 0.9;
            margin-bottom: 20px;
        }
        p{
            color:$SmallText;
            font-size:14px;
        }
    }
   .about{
        margin-left: 60%;
        padding-top: 150px ;
        color: white;
        padding-bottom: 30px;
    }
   .CTA{
        width: 90%;
        background-color: $Mygreen;
        padding: 70px;
        align-items: center;
   }
   .flexItem{
    width: 25%;
    margin-left: 150px;

    p{
        color:$SmallText;
        font-size: 11px;
    }
    h2{
        color:$BlueText;
        font-size: 26px;
    }
   }
</style>