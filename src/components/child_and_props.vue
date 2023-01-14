<template>
    <div class="child">
        <h1>Child Component</h1>
        <h3 v-for="user in users" :key="user.id">
            {{ user.name }}::
            {{ user.email }}
        </h3>
        <wazazi/>
    
    </div>
    
</template>

<script>
import wazazi from './props_parent_child.vue'
export default {
    name:"child",
    props:['name'],
    data(){
        return{
            users:[
                {name:"kev",email:"kev@gmail.com"},
                {name:"dave",email:"dave@gmail.com"},
                {name:"evans",email:"evans@gmail.com"}
            ]
    }  
    },
    components:{
        wazazi
    }
}
</script>

<style scoped>
.child{
background: purple;
width: 500px;
height: auto;
float: right;
margin-top: 20px;
color: gainsboro;
}
</style>