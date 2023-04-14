<template>
  <div class="lang-menu">
    <div class="drop-menu">
      <div class="menu-icon">
        <span
          ><img src="~/assets/images/arabc-flag.png" alt="arabc-flag"
        /></span>
        <span class="icon-chevron_down"></span>
      </div>

      <ul>
        <li>
          <div class="check-group">
            <input
              type="radio"
              name="header-check"
              id="lang-ar"
              class="check-radio-input"
              checked
            />
            <label class="check-label-radio" for="lang-ar">
              <span class="check-radio-button"></span>العربية - AR
            </label>
          </div>
        </li>
        <li>
          <div class="border-line"></div>
        </li>
        <li>
          <div class="check-group">
            <input
              type="radio"
              name="header-check"
              id="lang-en"
              class="check-radio-input"
            />
            <label class="check-label-radio" for="lang-en">
              <span class="check-radio-button"></span>English - EN
            </label>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "LangMenu",
  layout: "component",
};
</script>
