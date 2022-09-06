<template>
  <div class="containerfoot flex">
    <div class="box">
        <div id="getStarted">
            <h1>LET'S TALK ABOUT WORK</h1>
            <div class="testofoot">
                <p>A wonderful serenity has taken possession Far far away, behind the word mountains</p>
            </div>
            <button><a href="#">GET STARTED</a></button>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name:'MyFooter'
}
</script>

<style lang="scss" scoped>
.containerfoot{
    margin-top: 200px;
    background-image: url('../assets/foot.jpg');
    padding: 80px;
    color: white;
    justify-content: center;
    align-items: center;
    text-align: center;
}

.testofoot{
    width: 300px;
    text-align: center;
}
</style>