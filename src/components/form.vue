<template>      
    <div class="form">
    <h1>Form with checkbox and radio button in vue js</h1>
    <input type="text" v-model="signUpForm.username" placeholder="Enter your username" /><br/><br/>
    <input type="password" v-model="signUpForm.password" placeholder="Enter your password "/><br/><br/>
    <button>Submit</button>
    <br/>
    <br/>
    <div class="zingine">
    <p>Choose your course wisely</p>
    <br/>
    <input type="checkbox" v-model="signUpForm.courses" value="cs" id="cs"/>
    <label for="cs">Computer Science</label>
    <input type="checkbox" v-model="signUpForm.courses" value="pilot" id="pilot"/>
    <label for="pilot">Seller</label>
    <input type="checkbox" v-model="signUpForm.courses" value="eng" id="eng"/>
    <label for="eng">Engineer</label>
    <br/>
    <input type="radio" v-model="signUpForm.gender" value="male" id="male"/>
    <label for="male">Male</label>
    <br/>
    <input type="radio" v-model="signUpForm.gender" value="female" id="female"/>  
    <label for="female">Female</label>
    
   </div>
  
    </div>    
    <div>
    <button v-on:click="signUp">Sign up</button>
   
    </div>
</template>

<script>
export default {
    name:"signup",
    methods:{
        signUp(){
            console.log("This has been accepted",this.signUpForm)

        }
    },
    data()
    {
        return{
            signUpForm:{
                username:null,
                password:null,
                courses:[],
                gender:null

            }

        }
    }


}
</script>

<style scoped>
.form{
    color:black;
    font-size:20px;
    padding-left:20px;
}
 input[type=checkbox]{
    display: block;
    bottom: 1px;
    margin-left:300px;
    display: block;
    align-items: center;
    margin-top: 100px;
    
 }
 label{
    margin-top: 100px;
    align-items: center;


 }
</style>