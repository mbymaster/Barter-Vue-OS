<template>
  <div>
    <form class="form-register" v-on:submit.prevent="onSubmit">
      <h1 class="h3 mb-3 font-weight-normal">Sign up</h1>
      <div class="form-group">
        <label for="exampleInputEmail1">Email address</label>
        <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Enter email">
        <!-- <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone else.</small> -->
      </div>
      <div class="form-group">
        <label for="name">Name</label>
        <input type="text" class="form-control" id="name" aria-describedby="nameHelp" placeholder="Enter Name">
      </div>
      <div class="form-group">
        <label for="exampleInputPassword1">Password</label>
        <input type="password" class="form-control" id="inputPassword" placeholder="Password">
      </div>
      <div class="form-group">
        <label for="exampleInputPassword1">Verify Password</label>
        <input type="password" class="form-control" id="verifyPassword" placeholder="Verify Password">
      </div>
      <button type="submit" class="btn btn-primary" style="width: 100%;">Sign up</button>
    </form>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'SignupForm',
  methods: {
    onSubmit () {
      return 1
    }
  }
})
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
html,
body {
  height: 100%;
}

body {
  display: -ms-flexbox;
  display: flex;
  -ms-flex-align: center;
  align-items: center;
  padding-top: 40px;
  padding-bottom: 40px;
  background-color: #f5f5f5;
}

.form-register {
  width: 100%;
  max-width: 330px;
  padding: 15px;
  margin: auto;
}

.form-register .checkbox {
  font-weight: 400;
}

.form-register .form-control {
  position: relative;
  box-sizing: border-box;
  height: auto;
  padding: 10px;
  font-size: 16px;
}

.form-register .form-control:focus {
  z-index: 2;
}

.form-register input[type="email"] {
  margin-bottom: -1px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}

.form-register input[type="password"] {
  margin-bottom: 10px;
  border-top-left-radius: 0;
  border-top-right-radius: 0;
}
</style>
