<template>
    <div class="child">
        <h1>Child Component</h1>
        <h3 v-for="user in users" :key="user.id">
            {{ user.name }}::
            {{ user.email }}
        </h3>
        <h2 style="color:aqua">Child + parent relationship</h2>
        <h3>{{ title }}</h3>        
        <wazazi v-on:megatron="updatethisbutton"/>    
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
            ],
            title:"Last try"
    }  
    },
    components:{
        wazazi
    },

    methods:{
        updatethisbutton(title){
            this.title=title
        }
       
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