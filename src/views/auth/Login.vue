<template>
  <div class="container-sm" style="max-width: 400px;">
    <br/>
    <div class="auth-border">
      <LoginForm></LoginForm>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import LoginForm from '@/components/auth/LoginForm'

export default {
  name: 'Login',
  components: {
    LoginForm
  }
}
</script>

<style scoped lang="scss">
  .auth-border {
    border: 2px solid grey;
    border-radius: 20px;
  }
</style>
