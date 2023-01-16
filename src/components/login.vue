<template>
    <div>
        <input type="text" v-model="loginForm.username" placeholder="Enter your email" /><br/><br/>
        <input type="text" v-model="loginForm.password" placeholder="Enter your password"/><br/><br/>
        <button v-on:click="getLogin">Login</button>
    </div>
    
</template>

<script>
export default {
    name:"login",
    data(){
        return{
            loginForm:{
                username:null,
                password:null
            }
        }
    },
    methods:{
        getLogin(){
            console.log("You are logged in",this.loginForm.username,this.loginForm.password)
        }

    }    
}
</script>

<style scoped>

</style>