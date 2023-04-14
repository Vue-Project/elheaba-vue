<template>
  <section class="common-section">
    <div class="container">
      <div class="row">
        <div class="col-md-3">
          <div class="filter-list">
            <h3>Categories</h3>

            <ul class="menu">
              <li v-for="(menu, index) in menus" :key="index">
                <a
                  @click="
                    toggle(menu.id);
                    arrowToggle(menu);
                  "
                >
                  <i class="fa fa-chevron-right" :class="{ 'down': menu.isToggled, 'up': !menu.isToggled  }" ></i>
                  {{ menu.name }}
                </a>
                <div class="dropdown" v-show="menu.id === open">
                  <div v-for="(item, index) in menu.subMenu" :key="index">
                    <a to="#" class="options">
                      {{ item }}
                    </a>
                  </div>
                </div>
              </li>
            </ul>

            <h3>Price range</h3>

            <Slider v-model="value" :format="format" />
          </div>
        </div>
        <div class="col-md-9">
          <TheOffers />
          <ThePagnation />
        </div>
      </div>
    </div>
  </section>
</template>
<style lang="scss" scoped>
::v-deep {
  .down {
    transform: rotate(90deg);
  }
  .up {
    transform: rotate(0deg);
  }

  .slider-connects {
    background: #8b8b97;
  }
  .slider-tooltip {
    background: transparent;
    border: none;
    color: #8b8b97;
    font-size: 14px;
  }
  .slider-horizontal .slider-tooltip-top:before {
    border: none;
  }
  .slider-connect {
    background: #f89b26;
  }
  .slider-handle {
    background: #f89b26;
    border: 2px solid #ffffff;
    box-shadow: none;
  }
  .slider-horizontal .slider-tooltip-top {
    bottom: -22px;
  }
}
</style>

<script>
import Slider from "@vueform/slider/dist/slider.vue2.js";
import SliderStyle from "@vueform/slider/themes/default.css";

export default {
  name: "Categoriespage",
  layout: "main",
  components: {
    Slider,
    SliderStyle,
  },
  data() {
    return {
      value: [20, 80],
      format: function (value) {
        return `$${value}`;
      },
      open: null,
      isToggled: false,

      menus: [
        {
          id: 1,
          name: "Fruits",
          subMenu: [
            "Apple",
            "Grapes",
            "Orange",
            "Strawberry",
            "Pear-Kiwi",
            "Banana",
          ],
          isToggled: false,
        },
        {
          id: 2,
          name: "Dates",

          subMenu: [
            "Apple",
            "Grapes",
            "Orange",
            "Strawberry",
            "Pear-Kiwi",
            "Banana",
          ],
          isToggled: false,
        },
        {
          id: 3,
          name: " Food",

          subMenu: [
            "Apple",
            "Grapes",
            "Orange",
            "Strawberry",
            "Pear-Kiwi",
            "Banana",
          ],
          isToggled: false,
        },
        {
          id: 4,
          name: "Leaf ",

          subMenu: [
            "Apple",
            "Grapes",
            "Orange",
            "Strawberry",
            "Pear-Kiwi",
            "Banana",
          ],
          isToggled: false,
        },
        {
          id: 5,
          name: "Vegetables",

          subMenu: [
            "Apple",
            "Grapes",
            "Orange",
            "Strawberry",
            "Pear-Kiwi",
            "Banana",
          ],
          isToggled: false,
        },
        {
          id: 6,
          name: "Honey",

          subMenu: [
            "Apple",
            "Grapes",
            "Orange",
            "Strawberry",
            "Pear-Kiwi",
            "Banana",
          ],
          isToggled: false,
        },
      ],
    };
  },

  methods: {
    toggle(id) {
      this.open = this.open === id ? null : id;
    },
    arrowToggle(menu) {
      return (menu.isToggled = !menu.isToggled);
    },
    getItems() {
      return this.menus;
    },
  },
  mounted() {
    this.getItems();
  },
};
</script>
