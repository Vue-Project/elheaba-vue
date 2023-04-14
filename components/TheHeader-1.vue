<template>
  <header id="main-header" :class="mode">
    <nav class="navbar navbar-expand-lg">
      <div class="container">
        <!-- Brand -->
        <a class="navbar-brand" href="./index.html">
          <img src="~/assets/images/logo.png" class="navbar-brand-img" alt="Corptia Logo" />
        </a>

        <!-- Toggler -->
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarCollapse"
          aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>

        <!-- Collapse -->
        <div class="collapse navbar-collapse" id="navbarCollapse">
          <!-- Toggler -->
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarCollapse"
            aria-controls="navbarCollapse" aria-expanded="false" aria-label="Toggle navigation">
            <i class="fe fe-x"></i>
          </button>
i
          <!-- Navigation -->
          <ul class="navbar-nav m-auto">
            <li class="nav-item">
              <!-- <a class="nav-link" href="/" aria-haspopup="true" aria-expanded="false">
                Home
              </a> -->
              <NuxtLink class="nav-link" to="/">Home</NuxtLink>
            </li>
            <li class="nav-item">
              <!-- <a class="nav-link"  href="/company.html" aria-haspopup="true" aria-expanded="false">
                Company
              </a> -->
              <NuxtLink class="nav-link" to="/company">Company</NuxtLink>
            </li>
            <li class="nav-item">
              <!-- <a class="nav-link" href="/services.html" aria-haspopup="true" aria-expanded="false">
                Services
              </a> -->
              <NuxtLink class="nav-link" to="/services">Services</NuxtLink>
            </li>
            <li class="nav-item">
              <!-- <a class="nav-link" href="/works.html" aria-haspopup="true" aria-expanded="false">
                Works
              </a> -->
              <NuxtLink class="nav-link" to="/works">Works</NuxtLink>
            </li>
            <li class="nav-item">
              <!-- <a class="nav-link" id="navbarLandings"  href="/blog.html" aria-haspopup="true" aria-expanded="false">
                Blog
              </a> -->
              <NuxtLink class="nav-link" to="/blog">Blog</NuxtLink>
            </li>
            <li class="nav-item">
              <!-- <a class="nav-link" id="navbarLandings"  href="/contact.html" aria-haspopup="true" aria-expanded="false">
                Contact Us
              </a> -->
              <NuxtLink class="nav-link mr-0" to="/contact">Contact US</NuxtLink>
            </li>
          </ul>

          <!-- Button -->
          <SocialMedia />

        </div>
      </div>
    </nav>
    <ThePageHeader />

  </header>
</template>

<script>
import SocialMedia from '../components/SocialMedia.vue';

export default {
  components: {
    SocialMedia


  },
  name: "Header",
  props: {
    mode: {
      type: String,
    },
  },
};
</script>

<style>

</style>
