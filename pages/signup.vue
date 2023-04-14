<template>
  <div class="account-page">
  <form action="" class="signin-form">
    <a href="#"><img src="~/assets/images/logo.png" alt="" /></a>
    <h5>Sign Up</h5>

    <div class="row">
      <div class="col-md-6">
        <div class="form-group">
          <input class="form-control" type="text" placeholder=" First Name" />
        </div>
      </div>
      <div class="col-md-6">
        <div class="form-group">
          <input class="form-control" type="text" placeholder="Last Name" />
        </div>
      </div>
    </div>
    <div class="form-group">
      <input class="form-control" type="text" placeholder="Phone" />
    </div>
    <div class="form-group">
      <input class="form-control" type="text" placeholder="Email Address" />
    </div>
    <div class="form-group">
      <input class="form-control" type="password" placeholder="Password" />
      <a href="#"
        ><img class="password-hide" src="~/assets/images/pass-hide.svg" alt=""
      /></a>
    </div>
    <div class="row">
      <div class="col-md-4">
        <div class="form-group">
          <select class="form-control">
            <option selected>Day</option>
            <option value="1">One</option>
            <option value="2">Two</option>
            <option value="3">Three</option>
          </select>
        </div>
      </div>
      <div class="col-md-4">
        <div class="form-group">
          <select class="form-control">
            <option selected>Month</option>
            <option value="1">One</option>
            <option value="2">Two</option>
            <option value="3">Three</option>
          </select>
        </div>
      </div>
      <div class="col-md-4">
        <div class="form-group">
          <select class="form-control">
            <option selected>year</option>
            <option value="1">One</option>
            <option value="2">Two</option>
            <option value="3">Three</option>
          </select>
        </div>
      </div>
    </div>
    <div class="custom-control custom-checkbox">
      <input type="checkbox" class="custom-control-input" id="customCheck1" />
      <label class="custom-control-label" for="customCheck1"
        >Receive email updates and special promo offers?</label
      >
    </div>
    <button type="submit" class="btn-main btn-block">Create Account</button>


    <div class="account-about">
        <p>Already have an account?<span><a href="">Login here.</a></span></p>
    </div>
  </form>
</div>
  </template>
  
  <script>
  export default {
    name: "SignUpPage",
    layout: "page",
  };
  </script>
  