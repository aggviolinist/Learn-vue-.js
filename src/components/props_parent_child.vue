<template>
   <!-- <h3>{{ title }}</h3> --> 
  
    <button v-on:click="clickme">Please click me</button>
    
</template>

<script>
export default {
    name:"wazazi",
    components:{

    },
    data()
    {
        return{
            title:"Props, Child to Parent in vue "
        }
    },
    methods:{
        clickme()
        {
        //alert("I have been clicked")
        this.$emit('megatron','I changed coz you clicked me')

        }
        
    }
}
</script>

<style scoped>

</style>