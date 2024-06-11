<script>
export default {
    data() {
        return 
            {
        }
    }
}
</script>

<template>
    <div class="jumbotron">
    </div>
    <button>CURRENT SERIES</button>
    <div class="cards">

    </div>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables.scss' as *;
.jumbotron{
    width: 100%;
    height: 450px;
    background-image: url(../assets/img/jumbotron.jpg);
}
button{
    background-color: $active_color;
    color: white;
    padding: 1rem;
    font-size: 1.5rem;
    font-weight: bold;
    position: absolute;
    left: 20%;
    top: 45%;
}
.cards{
    background-color: $bg_main_color;
    width: 100%;
}
</style>