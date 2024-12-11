<template>
  <img src="../assets/logo.png" class="logo">
    <h1>Signup</h1>
    <div class="register">

      <input type="text" v-model="name" placeholder="Enter Name"/>
      <input type="text" v-model="email" placeholder="Enter Email"/>
      <input type="password" v-model="password" placeholder="Enter Password"/>

      <button v-on:click="signUp">Signup</button>

    </div>
  </template>
  
  <script>
  export default {
    name: 'SignUp',
    data(){
      return {
        name:'',
        email:'',
        password:''
      }
    },
    methods:{
      signUp(){
        console.warn("SignUp")
      }
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>

 .logo{
  width:100px;
 }

 .register input{
  width: 300px;
  height: 40px;
  padding-left: 20px;
  display: block;
  margin-bottom: 30px;
  margin-left: auto;
  margin-right: auto;
  border: 1px solid green;
 }

 .register  button{
  width: 320px;
  height: 40px;
  bottom: 1px solid green;
  color: white;
  background-color: green;
  cursor: pointer;
 }
  </style>
  