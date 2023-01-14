<template>
   <div class="rich">
    <p v-html="header">    
    </p>
        <h1>Home component</h1>
        <users />  <child users="users"/>
        <products/>  
        <databind/>
                  
    </div>  
</template>

<script>
import products from './products.vue'
import users from './users'
import databind from './databind.vue'
import child from './child.vue'

export default {
    rich:"compo",
    components:{
        users,
        products,
        databind,
        child

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
    height: 10000px;

}
</style>