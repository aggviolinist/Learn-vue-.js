<template>
    <div class="rich">
        <h1>Home component</h1>
        <users />
        <products/>
        
    </div>
    
</template>

<script>
import products from './products.vue'
import users from './users'
export default {
    rich:"compo",
    components:{
        users,
        products
        

        

    }
    
}
</script>

<style scoped>
.rich{
    background: red;
    height: auto;

}


</style>