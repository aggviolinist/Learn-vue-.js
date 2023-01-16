<template>
   <div class="rich">
    <p v-html="header">    
    </p>
        <h1>Home component</h1>
        <users />  <child users="users"/>
        <products/>  
        <databind/>
        <login/>
                  
    </div>  
</template>

<script>
import products from './products.vue'
import users from './users'
import databind from './databind.vue'
import child from './child_and_props.vue'
import login from './login.vue'

export default {
    rich:"compo",
    components:{
        users,
        products,
        databind,
        child,
        login

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