<template>
  <div>
    <section class="common-section">
    <TheCategory />
    <TheOffers/>
    <TheDiscounts/>
    <TheOffers/>
    <ThePageFooter/>
  </section>

    

     <u-animate-container>
      <u-animate
        name="fadeIn"
        delay="0s"
        duration="1s"
        :iteration="1"
        :offset="0"
        animateClass="animated"
        :begin="false"
      >
      </u-animate>
    </u-animate-container>
    <u-animate-container>
      <u-animate
        name="fadeIn"
        delay="0s"
        duration="2s"
        :iteration="1"
        :offset="0"
        animateClass="animated"
        :begin="false"
      >
        
      </u-animate>
    </u-animate-container> 
  </div>
</template>
<style scoped>
</style>

<script>
// mount with component
import { UAnimateContainer, UAnimate } from "vue-wow";
 export default {
  name: "IndexPage",
  layout: "main",
   components: {
    UAnimateContainer,
    UAnimate,
 
   },

  middleware: ["password-protect"],

  mounted() {
    this.$nextTick(() => {
      this.$nuxt.$loading.start();
      setTimeout(() => this.$nuxt.$loading.finish(), 2000);
    });
  },
  methods: {
    logout() {
      this.$passwordProtect.removeAuthorisation();
      this.$nextTick(() => {
        this.$router.push(this.localePath("password"));
      });
    },
  },
};
</script> 
