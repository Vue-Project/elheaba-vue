<template>
  <aside class="main-sidebar">
    <ul>
      <li>
        <nuxt-link
          exact-active-class="active"
          active-class="active"
          to="/account"
        >
          <i class="icon-person icon"> Account </i>
        </nuxt-link>
      </li>

      <li>
        <nuxt-link
          exact-active-class="active"
          active-class="active"
          to="/mylist"
        >
          <i class="icon-heart icon"> My List </i>
        </nuxt-link>
      </li>
      <li>
        <nuxt-link
          exact-active-class="active"
          active-class="active"
          to="/payment"
        >
          <i class="icon-payment icon"> Payment Methods </i>
        </nuxt-link>
      </li>
      <li>
        <nuxt-link
          exact-active-class="active"
          active-class="active"
          to="/adress"
        >
          <i class="icon-location"> Address </i>
        </nuxt-link>
      </li>
      <li>
        <nuxt-link
          exact-active-class="active"
          active-class="active"
          to="/myorder"
        >
          <i class="icon-clipboard"> My Order </i>
        </nuxt-link>
      </li>
      <li>
        <nuxt-link
          exact-active-class="active"
          active-class="active"
          to="/Setting"
        >
          <i class="icon-settings"> Setting</i>
        </nuxt-link>
      </li>
      <li>
        <nuxt-link exact-active-class="active" active-class="active" to="#">
          <i class="icon-logout"> Logout </i>
        </nuxt-link>
      </li>
    </ul>
  </aside>
</template>

<script>
export default {
  name: "TheSlidebar",
  layout: "component",
};
</script>

<style></style>
