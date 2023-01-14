<template>
    <div>
        <p v-html="header">
            
        </p>
    <h1>Templates in vue js</h1>
    <h2>{{ name }}</h2>
    <h2 v-once>{{ name }}</h2>
    <button v-bind:disabled="btndisabled" v-on:click="hello">Click me</button>
    <h3>{{ ok?"yes":"no" }}</h3>
    </div>
       
</template>

<script>
export default {
    name:"template",
    data(){
        return{
            name:"violinist",
            ok:true,
            btndisabled:true
           
        }
    },
    methods:{//property
        hello()
        {
            alert("Hello click")
            //this.name="aggressive"
            this.ok=false            
        }
    }
}
</script>
<style scoped>
h1{
    color:black;
}
h2{
    color:gold
}
</style>
