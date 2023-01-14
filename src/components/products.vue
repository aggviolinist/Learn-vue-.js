<template>
    <div class="products">
        <h2>Products Component</h2>
        <name/> 
    </div>
</template>

<script>
import name from './template.vue'
export default{
    rich:"products",
    components:{
        name
    }
}
</script>

<style scoped>
.products{
background: blue;
width: 500px;
height: 250px;
padding: 80px;
margin: 50px;
}
</style>