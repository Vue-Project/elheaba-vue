<template>
  <section class="common-section">
    <div class="container">
      <div class="contact-section">
        <div class="row">
          <div class="col-md-6">
            <form action="" class="contact-form">
              <h1 class="section-title">Contact Us</h1>
              <div class="form-group">
                <input
                  class="form-control"
                  type="text"
                  placeholder="Name"
                  id="user-name"
                  name="user-name"
                />
              </div>
              <div class="form-group">
                <input
                  class="form-control"
                  type="text"
                  placeholder="Email"
                  id="user-email"
                  name="user-email"
                />
              </div>
              <div class="form-group">
                <input
                  class="form-control"
                  type="text"
                  placeholder="Title"
                  id="user-titel"
                  name="user-titel"
                />
              </div>
              <div class="form-group">
                <textarea
                  class="form-control form-textarea"
                  placeholder="Message"
                  id="user-massage"
                  name="user-massage"
                ></textarea>
              </div>
              <button type="submit" class="btn-main btn-block">Send</button>
            </form>
          </div>
          <div class="col-md-6">
            <div class="contact-infro">
              <h1 class="section-title">Info</h1>
              <h5>Adress</h5>
              <p>26/C Mohammadpur Dhaka, Bangladesh</p>
              <h5>Phone</h5>
              <p>+91 123 456 789</p>
              <h5>Email</h5>
              <p>Alheba@gmail.com</p>

              <h5>Social Media</h5>
              <SocialMedia />
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ContactPage",
  layout: "main",
};
</script>
