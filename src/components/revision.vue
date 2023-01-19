<template>
    <div>
        <hr/>
        <h1 >Revision on form validation</h1>
        <hr/>
        <p v-if="error.length">
            <b>Please correct these errors</b>
            <ul>
                <li v-for="e in error" v-bind:key="e.id">
                {{ e }}
                </li>
            </ul>

        </p>
        
            
        <form @submit="LoginRev">
            <input type="text" v-model="username" placeholder="Enter your username"/><br/><br/>
            <input type="text" v-model="password" placeholder="Enter your password"/><br/><br/>
            <button type="submit">Click me to submit</button>
        </form>

    </div>


</template>


<script>
export default {
    name:"revisionLogin",
    methods:{
        LoginRev(e){
            if(this.username && this.password)
            {
            console.log("Info submitted")

            }
            this.error=[];
            if(!this.username)
            {
                this.error.push("Please enter a username")
            }
            if(!this.password)
            {
                this.error.push("Please enter a password")
            }
            console.warn("there are a couple errors",this.error)
            
            e.preventDefault()

        }},
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
h1{
    color:chartreuse;
}

</style>