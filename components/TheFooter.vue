<template>
  <footer class="footer-section">
    <div class="container">
      <div class="footer-content">
        <div class="row">
          <div class="col-lg-3 col-md-6 col-sm-6">
            <div class="logo-footer">
              <a class href="#"
                ><img src="~/assets/images/logo.png" alt="logo-image"
              /></a>
            </div>
            <ul>
              <li>
                <span> <i class="fas fa-map-marker-alt"></i></span>

                <p>Headley Ln, Dorking</p>
              </li>
              <li>
                <span> <i class="fa fa-phone"></i></span>
                <p>+91 123 456 789</p>
              </li>
              <li>
                <span><i class="far fa-envelope"></i></span>
                <p>Alheba@gmail.com</p>
              </li>
            </ul>
            <SocialMedia />
          </div>
          <div class="col-lg-3 col-md-6 col-sm-6">
            <ul>
              <h6>Site Map</h6>
              <li>
                <a href="/categories">Category</a>
              </li>
              <li>
                <a href="/mylist">My List</a>
              </li>
              <li>
                <a href="/payment">Payment Methods</a>
              </li>
              <li>
                <a href="/myorder">My Order</a>
              </li>
            </ul>
          </div>
          <div class="col-lg-3 col-md-6 col-sm-6">
            <ul>
              <h6>About us</h6>
              <li>
                <a href="/about-us">About the company</a>
              </li>
              <li>
                <a href="#">Branches</a>
              </li>
              <li>
                <a href="#">FAQ</a>
              </li>
              <li>
                <a href="#">Our App</a>
              </li>
            </ul>
          </div>
          <div class="col-lg-3 col-md-6 col-sm-6">
            <ul>
              <h6>Support</h6>
              <li>
                <a href="/contact">Contact us</a>
              </li>
              <li>
                <a href="/privacy">Privacy policy</a>
              </li>
              <li>
                <a href="/conditions">Terms and Conditions</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
      <p class="copyright">
        Copyright © 2021 AlHeba All Rights Reserved Made by Corptia
      </p>
    </div>
  </footer>
</template>

<script>
import SocialMedia from "./SocialMedia.vue";
export default {
  components: {
    SocialMedia,
  },
};
</script>

<style></style>
