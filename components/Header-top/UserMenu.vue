<template>
  <div class="account-option">
    <div class="drop-menu">
      <div class="menu-icon">
        <span
          ><img src="~/assets/images/icon-person.svg" alt="icon-person"
        /></span>
        <p class="name-user">Hello, Mona</p>
        <span class="icon-chevron_down"></span>
      </div>

      <ul>
        <li>
          <a
            exact-active-class="active"
            active-class="active"
            href="/account"
          >
            <i class="icon-person"> Account </i>
          </a>
        </li>
        <li>
          <div class="border-line"></div>
        </li>
        <li>
          <a exact-active-class="active" active-class="active" href="/mylist">
            <i class="icon-heart"> My List </i>
          </a>
        </li>
        <li>
          <div class="border-line"></div>
        </li>
        <li>
          <a exact-active-class="active" active-class="active" href="/payment">
            <i class="icon-payment"> Payment Methods </i>
          </a>
        </li>
        <li>
          <div class="border-line"></div>
        </li>
        <li>
          <a exact-active-class="active" active-class="active" href="/adress">
            <i class="icon-location"> Address </i>
          </a>
        </li>

        <li>
          <div class="border-line"></div>
        </li>
        <li>
          <a exact-active-class="active" active-class="active" href="/myorder">
            <i class="icon-clipboard"> My Order </i>
          </a>
        </li>

        <li>
          <div class="border-line"></div>
        </li>
        <li>
          <a exact-active-class="active" active-class="active" href="/setting">
            <i class="icon-settings"> Setting </i>
          </a>
        </li>
        <li>
          <div class="border-line"></div>
        </li>
        <li>
          <a exact-active-class="active" active-class="active" href="/logout">
            <i class="icon-logout"> logout </i>
          </a>
        </li>
      </ul>
      
    </div>
  </div>
</template>

<script>
export default {
  name: "UserMenu",
  layout: "component",
};
</script>

<style></style>
