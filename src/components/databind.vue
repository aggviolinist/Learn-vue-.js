<template>
    <div class="bind">
        <h1>Bind Component</h1>
        <h2 style="white-space:pre-line">{{ message }}</h2>
        <input type="text" v-model="message"/>
        <br/>
        <br/>
        <textarea type="text" v-model="message"/>
    </div>
</template>

<script>
export default{
    name:"homeBind",
    data()
    {
        return{
            message:"Hi I'm excited learning this stuff"
        }
    }
}
</script>

<style>
.bind{
background: yellow;
width: 500px;
height: auto;
padding: 80px;
margin: 50px;
}
</style>