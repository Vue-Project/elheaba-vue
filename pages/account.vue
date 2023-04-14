<template>
  <section class="common-section">
    <div class="container">
      <div class="row">
        <div class="col-md-3">
            <Theslidebar/>
        </div>
        <div class="col-md-9">
          <h1 class="section-title">Account</h1>
          <div class="data-box">
            <div class="box-head">
              <p>
                You completed your registration successfully<span>100%</span>
              </p>
            </div>
            <div class="box-content">
              <h5>Mona Mostafa <a href="">Edit</a></h5>
              <div class="customer-data">
                <div class="item-data">
                  <img src="~/assets/images/data-icon.1.png" alt="" />

                  <div class="item-infro">
                    <span>Email</span>
                    <p>Mona@gmail.com</p>
                  </div>
                </div>
                <div class="item-data">
                  <img src="~/assets/images/data-icon.2.png" alt="" />

                  <div class="item-infro">
                    <span>Phone</span>
                    <p>+91 123 456 789</p>
                  </div>
                </div>
                <div class="item-data">
                  <img src="~/assets/images/data-icon.3.png" alt="" />

                  <div class="item-infro">
                    <span>Date of birth</span>
                    <p>1 / 6 / 1999</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div class="row">
            <div class="col-lg-6 col-md-12">
              <h1 class="section-title">Adress <a href="#">See All</a></h1>

              <div class="data-box">
                <div class="box-content">
                  <h5>Home</h5>
                  <p>01063987432</p>
                  <p>26/C Mohammadpur Dhaka, Bangladesh</p>
                </div>
              </div>
            </div>
            <div class="col-lg-6 col-md-12">
              <h1 class="section-title">
                Payment Methods <a href="#">See All</a>
              </h1>

              <div class="data-box">
                <div class="box-content">
                  <h5>Master Card</h5>
                  <p>**** **** **** 4986</p>
                  <p>Exp. 18 /5</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
  
  <script>
  import Theslidebar from"../components/TheSidebar.vue"
export default {
  name: "AccountPage",
  layout: "main",
  components:{
    Theslidebar
  }
};
</script>
  