<template>
   <div class="rich">
    <p v-html="header">    
    </p>
        <h1>Home component</h1>
        <users />  <child users="users"/>
        <products/>  
        <databind/>
        <login/>
        <signup/>
        <validation/>
        <revisionLogin/>
        <formchannge/>
                  
    </div>  
</template>

<script>
import products from './products.vue'
import users from './users'
import databind from './databind.vue'
import child from './child_and_props.vue'
import login from './login.vue'
import signup from './form.vue'
import validation from './validation.vue'
import revisionLogin from './revision.vue'
import Formchannge from './formchannge.vue'

export default {
    rich:"compo",
    components:{
        users,
        products,
        databind,
        child,
        login,
        signup,
        validation,
        revisionLogin,
        Formchannge


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