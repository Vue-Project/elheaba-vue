<template>
  <div class="account-page">
    <form action="#" class="signin-form">
      <a href="#"><img src="~/assets/images/logo.png" alt="" /></a>
      <h5>Login</h5>

      <div class="form-group">
        <input class="form-control" type="text" placeholder="Phone" />
      </div>

      <div class="form-group">
        <input class="form-control" type="password" placeholder="Password" />
        <a href="#"
          ><img
            class="password-hide"
            src="~/assets/images/pass-hide.svg"
            alt=""
        /></a>
      </div>
      <div class="custom-control custom-checkbox">
        <input type="checkbox" class="custom-control-input" id="customCheck1" />
        <label class="custom-control-label" for="customCheck1">
          Remember me
        </label>
        <div class="forgot-password">
          <a href="">Forgot Password</a>
        </div>
      </div>

      <button type="submit" class="btn-main btn-block">Login</button>

      <div class="account-about">
        <p>
          Don't have an account?<span><a href="">Sign up here. </a></span>
        </p>
      </div>
    </form>
  </div>
</template>

<script>
export default {
  name: "SignInPage",
  layout: "page",
};
</script>
