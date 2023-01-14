<template>
    <h3>{{ heading }}</h3>
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
            heading:"Props, Child to Parent in vue "
        }
    },
    methods:{
        clickme()
        {
        alert("I have been clicked")

        }
        
    }
}
</script>

<style scoped>

</style>