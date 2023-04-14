<template>
  <div class="container">
    <h1 class="section-title">Category</h1>
    <vueper-slides
      autoplay
      class="no-shadow"
      :arrows="false"
      :visible-slides="6"
      slide-multiple
      :gap="3"
      :dragging-distance="3"
      :breakpoints="{ 800: { visibleSlides: 2, slideMultiple: 2 } }"
    >
      <vueper-slide
        v-for="slide in slides"
        :key="slide.id"
        :image="slide.image"
      />
      <!-- <p :title="slide.title"></p> -->
    </vueper-slides>
  </div>
</template>

<script>
import "vueperslides/dist/vueperslides.css";

import { VueperSlides, VueperSlide } from "vueperslides";

export default {
  name: "TheCategory",
  layout: "component",

  components: {
    VueperSlides,
    VueperSlide,
  },

  data() {
    return {
      slides: [
        {
          image: require("~/assets/images/categorys/category-01.png"),
        },
        {
          image: require("~/assets/images/categorys/category-02.png"),
        },
        {
          image: require("~/assets/images/categorys/category-03.png"),
        },
        {
          image: require("~/assets/images/categorys/category-04.png"),
        },
        {
          image: require("~/assets/images/categorys/category-05.png"),
        },
        {
          image: require("~/assets/images/categorys/category-06.png"),
        },
        {
          image: require("~/assets/images/categorys/category-01.png"),
        },
        {
          image: require("~/assets/images/categorys/category-02.png"),
        },
        {
          image: require("~/assets/images/categorys/category-03.png"),
        },

        {
          image: require("~/assets/images/categorys/category-04.png"),
        },

        {
          image: require("~/assets/images/categorys/category-05.png"),
        },

        {
          image: require("~/assets/images/categorys/category-06.png"),
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
::v-deep {
  .vueperslides__track {
    height: 50%;
  }

  .vueperslides__inner {
    height: 200px;
  }
  .vueperslides__bullet--active .default {
    background: #f89b26;
    border-color: #f89b26;
    box-shadow: none;
  }
  .vueperslides__bullet .default {
    border-color: #f89b26;
    box-shadow: none;
  }
}
</style>
