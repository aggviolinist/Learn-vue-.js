<template>
    <div class="users"> 
        <h1>Users Component</h1>
        <classes></classes>
     </div>      
</template>

<script>
import classes from './classes.vue'
export default {
    rich:"users",
    components:{
        classes

    }    
}
</script>

<style scoped>
.users{
background: green;
width: 500px;
height: 200px;
padding: 80px;
margin: 50px;
}
</style>