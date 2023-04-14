<template>
  <div>
    <TheHeader />
    <ThePageHeader />
    <Nuxt />
    <!-- <CursorFx color="#001560" color-hover="#f1c40f" /> -->
    <TheFooter />
  </div>
</template>

<script>
import { CursorFx } from "@luxdamore/vue-cursor-fx";

export default {
  components: { CursorFx },
};
</script>

<style src="@luxdamore/vue-cursor-fx/dist/CursorFx.css"></style>
