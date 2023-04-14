<template>
  <section class="common-section">
    <div class="container">
      <div class="row">
        <div class="col-md-3">
          <Theslidebar />
        </div>
        <div class="col-md-9">
          <h1 class="section-title">Setting</h1>
          <form action="#" class="settiing-form">
            <div class="row">
              <div class="col-md-6">
                <div class="form-group">
                  <label for="user-name"> frist Name</label>

                  <input
                    class="form-control"
                    type="text"
                    placeholder=" First Name"
                    id="user-frist"
                  />
                </div>
              </div>
              <div class="col-md-6">
                <div class="form-group">
                  <label for="user-email">last Name</label>

                  <input
                    class="form-control"
                    type="text"
                    placeholder="Last Name"
                    id="user-last"
                  />
                </div>
              </div>
            </div>
            <div class="form-group">
              <label for="user-email">Email</label>

              <input
                class="form-control"
                type="text"
                placeholder="Mona@gmail.com "
                id="user-email"
              />
            </div>
            <div class="form-group">
              <label for="user-number">Phone Number</label>

              <input
                class="form-control"
                type="number"
                placeholder="+91 123 456 789"
                id="user-number"
              />
            </div>
            <div class="form-group">
              <label for="user-password">Password </label>
              <span><a href="#">Change Password</a></span>

              <input class="form-control" type="password" id="user-password" />
            </div>

            <button type="submit" class="btn-main btn-block">Save</button>
          </form>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Theslidebar from "../components/TheSidebar.vue";
export default {
  name: "SettingPage",
  layout: "main",
  components: {
    Theslidebar,
  },
};
</script>
