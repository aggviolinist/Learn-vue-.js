<template>
    <div>
        <hr/>
        <hr/>
        <h1>this is it</h1>
        <h1>{{ name }}</h1>
        <h2 id="demo">Mount or before mount</h2>
        <h2>Create or before create</h2>
        <h2 v-if="display">Destroy or before destroy</h2>
        <button v-on:click="toogle">Toggle and destroy</button>
    </div>
    
</template>

<script>


export default {
    name:"formchange",
    data()
    {
        return{
            name:"I'm kelvin and I'm learning vue:)",
            
            display:true
        
        }
    },
    methods:
    {
        toogle()
        {
            this.display=!this.display

        }
    },
    /**  -------------------++++++++++++MOUNT LIFECYCLE+++++++++++----------------------------
    beforeMount()
    {
        console.warn("before mount",this.$el)
    },
    mounted()
    {
        console.warn("mounted",this.$el)

    }
    *//** 
   beforeMount(){
    console.warn("before mount",document.getElementById("demo"))

   },
   mounted(){
    console.warn("mounted",document.getElementById("demo"))

   }
   */
    /** -------------------++++++++++++CREATE LIFECYCLE+++++++++++----------------------------
    beforeCreate()
    {
        console.warn("acha tucheki if itakua first",this.name)


    },
    beforeCreate()
    {
        this.name="before create "
        console.warn("before create ndio first",this.name)
    },
    created()
    {
        //this.name="lampz"
        console.warn("created",this.name)
    }
    */
    /**  does't do was suppose to be a capitalizing filter
    filters: {
     capitalize: function (value) {
    if (!value) return ''
    value = value.toString()
    return value.charAt(0).toUpperCase() + value.slice(1)
  }
}
*/
/** -------------------++++++++++++CREATE LIFECYCLE+++++++++++---------------------------- */
beforeUnmount()
{
    alert("Before the destruction method is called")

},
unmounted(){
    alert("After the destruction method is called last")

}


    
}
</script>

<style scoped>

</style>