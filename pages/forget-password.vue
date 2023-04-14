<template>
  <div class="account-page">
    <form action="" class="signin-form">
      <a href="#"><img src="~/assets/images/logo.png" alt="" /></a>
      <h5>Forgot The Password</h5>
      <p>Enter your phone number to reset password</p>

      <div class="form-group">
        <input class="form-control" type="text" />
      </div>

      <button type="submit" class="btn-main btn-block">
        Send security code
      </button>
    </form>
  </div>
</template>

<script>
export default {
  name: "ForgetPasswordPage",
};
</script>
