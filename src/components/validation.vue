<template>
    <div>
      <h2>Register</h2>
      <form @submit.prevent="register">
        <div>
          <label>Username:</label>
          <input type="text" v-model.trim="registerForm.username">
          <div v-show="!$v.registerForm.username.required">Username is required</div>
        </div>
        <div>
          <label>Email:</label>
          <input type="email" v-model.trim="registerForm.email">
          <div v-show="!$v.registerForm.email.required">Email is required</div>
          <div v-show="!$v.registerForm.email.email">Invalid email format</div>
        </div>
        <div>
          <label>Password:</label>
          <input type="password" v-model.trim="registerForm.password">
          <div v-show="!$v.registerForm.password.required">Password is required</div>
          <div v-show="!$v.registerForm.password.minLength">Password must be at least 8 characters long</div>
        </div>
        <div>
          <button type="submit" :disabled="$v.registerForm.$invalid">Register</button>
        </div>
      </form>
      
      <h2>Login</h2>
      <form @submit.prevent="login">
        <div>
          <label>Email:</label>
          <input type="email" v-model.trim="loginForm.email">
          <div v-show="!$v.loginForm.email.required">Email is required</div>
          <div v-show="!$v.loginForm.email.email">Invalid email format</div>
        </div>
        <div>
          <label>Password:</label>
          <input type="password" v-model.trim="loginForm.password">
          <div v-show="!$v.loginForm.password.required">Password is required</div>
        </div>
        <div>
          <button type="submit" :disabled="$v.loginForm.$invalid">Login</button>
        </div>
      </form>
    </div>
  </template>
  
  <script>
  import { required, email, minLength } from 'vuelidate/lib/validators'
  
  export default {
    name: 'FormValidation',
    data() {
      return {
        registerForm: {
          username: '',
          email: '',
          password: ''
        },
        loginForm: {
          email: '',
          password: ''
        }
      }
    },
    validations: {
      registerForm: {
        username: {
          required
        },
        email: {
          required,
          email
        },
        password: {
          required,
          minLength: minLength(8)
        }
      },
      loginForm: {
        email: {
          required,
          email
        },
        password: {
          required
        }
      }
    },
    methods: {
      register() {
        // Perform registration logic here
      },
      login() {
        // Perform login logic here
      }
    }
  }
  </script>
  