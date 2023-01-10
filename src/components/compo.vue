<template>
   <div class="rich">
    <p v-html="header">    
    </p>
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
        products,
        
    },
    data()
    {
        return{
            header:"<h1>enjoying this ting</h1>"

        }
    }    
}
</script>

<style scoped>
.rich{
    background: red;
    height: auto;

}
</style>