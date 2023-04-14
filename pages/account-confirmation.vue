<template>
    <div class="account-page">
  <form
    method="get"
    class="digit-group signin-form"
    data-group-name="digits"
    data-autosubmit="false"
    autocomplete="off"
  >
    <a href="#"><img src="~/assets/images/logo.png" alt="" /></a>
    <h5>Account Confirmation</h5>
    <p>Enter the 6 digit PIN that we sent to:</p>
    <p class="phone-number">+201*******010</p>
    <div class="digit-items">
      <div class="digit-item">
        <input type="text" id="digit-1" name="digit-1" data-next="digit-2" />
      </div>
      <div class="digit-item">
        <input
          type="text"
          id="digit-2"
          name="digit-2"
          data-next="digit-3"
          data-previous="digit-1"
        />
      </div>
      <div class="digit-item">
        <input
          type="text"
          id="digit-3"
          name="digit-3"
          data-next="digit-4"
          data-previous="digit-2"
        />
      </div>
      <div class="digit-item">
        <input
          type="text"
          id="digit-4"
          name="digit-4"
          data-next="digit-5"
          data-previous="digit-3"
        />
      </div>
      <div class="digit-item">
        <input
          type="text"
          id="digit-4"
          name="digit-4"
          data-next="digit-5"
          data-previous="digit-3"
        />
      </div>
      <div class="digit-item mr-0">
        <input
          type="text"
          id="digit-4"
          name="digit-4"
          data-next="digit-5"
          data-previous="digit-3"
          
        />
      </div>
    </div>
    <button type="submit" class="btn-main btn-block">Verify</button>
  </form>
</div>
  </template>
  
  <script>
  export default {
    name: "AccountConfirmationPage",
    layout: "page",
  };
  </script>
  