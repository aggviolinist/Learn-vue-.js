<template>
    <h3 class="vuestyle">Class and style Bindings</h3>
    <h2 v-bind:style="{color:'skyblue'}">Styling using vue js</h2>
    <h4 v-bind:class="[checkDisplay?v:d]">Classes with arrays</h4>
    <!--<h5 v-bind:class="[v]">Summer love</h5> -->
    
</template>

<script>
export default {
    rich:"classes",
    data(){
    return{
        d:"display",
        v:"yow",
        checkDisplay:true
    }
}    
}
</script>

<style scoped>
.vuestyle{
    color:olive

}
.display{
    background-color: pink;
    color: aqua;
    width: 200px;
    height: 10px;
    padding: 20px;
    margin-left: 200px;
}
.yow{
    background-color: chocolate;
    width: 100px;
    height:20px;
}
</style>