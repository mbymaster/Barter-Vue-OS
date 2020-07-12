<template>
  <div class="container-sm" style="max-width: 400px;">
    <br />
    <div class="auth-border">
      <SignupForm></SignupForm>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import SignupForm from "@/components/auth/SignupForm";

export default {
  name: "Login",
  components: {
    SignupForm
  }
};
</script>

<style scoped lang="scss">
.auth-border {
  border: 2px solid grey;
  border-radius: 20px;
}
</style>
