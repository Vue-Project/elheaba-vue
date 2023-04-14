<template>
  <header class="main-header">
    <div class="header-top">
      <div class="container">
        <div class="row center">
          <div class="col-lg-2 col-md-12">
            <a class="logo-header" href="/"
              ><img src="~/assets/images/logo.png" alt="logo-image"
            /></a>
          </div>
          <div class="col-lg-6 col-md-6">
            <form class="form-inline">
              <input
                class="form-control mb-0"
                type="search"
                placeholder="Search"
              />
              <a href=""><i class="fa fa-search" aria-hidden="true"></i></a>
            </form>
          </div>
          <div class="col-lg-4 col-md-6">
            <div class="header-top-right">
              <LangMenu />
              <UserMenu />
              <NotificationMenu />

              <span class="cart-icon">
                <a href="/cart"><img src="~/assets/images/cart-icon.svg" alt="cart-icon" /></a
              ></span>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="header-bottom">
      <div class="container">
        <nav class="navbar navbar-expand-lg">
          <a href="#" class="navbar-brand">menu</a>
          <button
            class="navbar-toggler"
            type="button"
            data-toggle="collapse"
            data-target="#navbarNav"
            aria-controls="navbarNav"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <span class="navbar-toggler-icon"></span>
          </button>

          <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav">
              <li class="nav-item active">
                <a class="nav-link" href="#">Honey</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">Dates</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">Food</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">Fruits</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">leaf vegetable</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#">Vegetables</a>
              </li>
            </ul>
          </div>
        </nav>
      </div>
    </div>
  </header>
</template>

<script>
import LangMenu from "../components/Header-top/LangMenu.vue"
import UserMenu from "../components/Header-top/UserMenu.vue"
import NotificationMenu from "../components/Header-top/NotificationMenu.vue"
export default {
  name: "Header",
  layout: "component",
  components:{
    LangMenu,
    UserMenu,
    NotificationMenu

  }
};
</script>


<style>
</style>