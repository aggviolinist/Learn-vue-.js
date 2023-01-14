<template>
    <div class="child">
        <h1>Child Component</h1>
        <h3 v-for="user in users" :key="user.name">
            {{ user.name }}::
            {{ user.email }}
        </h3>
    
    </div>
    
</template>

<script>
export default {
    name:"kido",
    props:['name'],
    data(){
        return{
            users:[
                {name:"kev",email:"kev@gmail.com"},
                {name:"dave",email:"dave@gmail.com"},
                {name:"evans",email:"evans@gmail.com"}
            ]
    }  
}
}
</script>

<style scoped>
.child{
background: purple;
width: 500px;
height: 250px;
float: right;
margin-top: 20px;
color: gainsboro;
}
</style>