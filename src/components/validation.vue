<template>
    <div>
    <hr/>
    <hr/>
    <h1>Login buttton mheeeen with validation</h1>
    <p v-if="error.length">
        <b>Please correct the following errors</b>
        <ul>
            <li v-for="e in error" v-bind:key="e.id">
                {{ e }}
            
            </li>
        </ul>

    </p>





    <p v-if="error.length">
            <b>Please correct these errors</b>
            <ul>
                <li v-for="e in error" v-bind:key="e.id">
                {{ e }}
                </li>
            </ul>
        </p>
        <form @submit="login">
            <input type="text" placeholder="Enter the username" v-model="username"/>
            <br/>
            <br/>
            <input type="text" placeholder="Enter the password" v-model="password"/>
            <br/>
            <br/>
            <button type="submit">Login</button>

        </form>
    </div>
    
</template>

<script>
export default {
    name:"validation",
    methods:{
        login(e){
            if(this.username && this.password)
            {           
            alert("login function has been called")
            }
            this.error=[];
            if(!this.username)
            {
                this.error.push("username is required")
            }
            if(!this.password)
            {
                this.error.push("Password is required")
            }
            console.warn("errors",this.error)
            e.preventDefault()
            
        }
    },
    data(){
        return{
            error:[],
            username:null,
            password:null
        }
    }
    
}
</script>

<style scoped>

</style>