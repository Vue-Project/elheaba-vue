<template>
  <section class="common-section">
    <div class="container">
      <div class="single-section">
        <div class="row">
          <div class="col-md-6">
            <vueper-slides
              ref="vueperslides1"
              :arrows="false"
              :touchable="false"
              fade
              :autoplay="false"
              :bullets="false"
              @slide="
                $refs.vueperslides2.goToSlide($event.currentSlide.index, {
                  emit: false,
                })
              "
              fixed-height="400px"
            >
              <vueper-slide
                v-for="(slide, i) in slides"
                :key="i"
                :image="slide.image"
              >
              </vueper-slide>
            </vueper-slides>

            <vueper-slides
              class="no-shadow thumbnails"
              ref="vueperslides2"
              @slide="
                $refs.vueperslides1.goToSlide($event.currentSlide.index, {
                  emit: false,
                })
              "
              :visible-slides="slides.length"
              fixed-height="75px"
              :bullets="false"
              :touchable="false"
              :gap="2.5"
              :arrows="false"
            >
              <vueper-slide
                v-for="(slide, i) in slides"
                :key="i"
                :image="slide.image"
                @click.native="$refs.vueperslides2.goToSlide(i)"
              >
              </vueper-slide>
            </vueper-slides>
          </div>
          <div class="col-md-6">
            <div class="dislike">
              <a href="">
                <i class="fa fa-heart-o" aria-hidden="true"></i>
              </a>
            </div>
            <h1>Tomatoes</h1>
            <span>1 KG</span>
            <div class="pricing">
              <p class="new-price">11.99 KDW</p>
              <del class="old-price">14.63 KDW</del>
            </div>
            <h6>Product Detailes</h6>
            <span
              >Lorem Ipsum is simply dummy text of the printing and typesetting
              industry</span
            >

            <div class="rating-star">
              <h6>Review</h6>
              <span class="fa fa-star checked"></span>
              <span class="fa fa-star checked"></span>
              <span class="fa fa-star checked"></span>
              <span class="fa fa-star checked"></span>
              <span class="fa fa-star"></span>
              <span class="number-reviews"><a href="">54 Reviews</a></span>
            </div>
            <h6>Quantity</h6>

            <div class="item-add">
              <button class="value-button decrease-button">
                <i class="fa fa-minus" aria-hidden="true"></i>
              </button>
              <div class="items-number">2</div>
              <button class="value-button increase-button">
                <i class="fa fa-plus" aria-hidden="true"></i>
              </button>
            </div>

            <button type="submit" class="btn-main btn-block">
              <i class="fa fa-shopping-cart" aria-hidden="true"></i>

              Add to bag
            </button>
          </div>
        </div>
      </div>
      <div class="seller-section">
        <div class="seller-content">
          <h1 class="section-title">Best seller</h1>

          <div class="row">
            <div
              class="col-lg-3 col-md-4 col-sm-6"
              v-for="offer in offers"
              :key="offer.id"
            >
              <div class="item-box">
                <div class="image-item">
                  <div class="dislike">
                    <a href="">
                      <i class="fa fa-heart-o" aria-hidden="true"></i>
                    </a>
                  </div>
                  <img :src="getImgUrl(offer.image)" :alt="offer.alt" />
                </div>
                <div class="item-details">
                  <h4>{{ offer.title }}</h4>
                  <p>{{ offer.des }}</p>
                  <p class="new-price">$10.99</p>
                  <del class="old-price">$24.99</del>
                </div>
                <button type="submit" class="btn-main btn-block">
                  <i class="fa fa-shopping-cart" aria-hidden="true"></i>

                  Add to bag
                </button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<style lang="scss" scoped>
::v-deep {
  .vueperslides {
    margin-bottom: 15px;
  }
  .thumbnails {
    margin: auto;
    max-width: 400px;
  }

  .thumbnails .vueperslide {
    box-sizing: border-box;
    border: 1px solid #fff;
    transition: 0.3s ease-in-out;
    opacity: 0.7;
    cursor: pointer;
  }

  .thumbnails .vueperslide--active {
    box-shadow: 0 0 6px rgba(0, 0, 0, 0.3);
    opacity: 1;
    border-color: #f89b26;
  }
}
</style>

<script>
import "vueperslides/dist/vueperslides.css";

import { VueperSlides, VueperSlide } from "vueperslides";
export default {
  name: "SingelProductPage",
  layout: "main",
  components: {
    VueperSlides,
    VueperSlide,
  },
  data() {
    return {
      slides: [
        { image: require("~/assets/images/image-gallery.png") },
        { image: require("~/assets/images/image-gallery.png") },
        { image: require("~/assets/images/image-gallery.png") },
        { image: require("~/assets/images/image-gallery.png") },
      ],
      offers: [
        {
          id: 1,
          image: "offers/offer-02.png",
          title: "Psoriasis Cream",
          des: "All Natural Ingredients.",
          alt: "Psoriasis Cream",
        },
        {
          id: 2,
          image: "offers/offer-03.png",
          title: "Psoriasis Cream",
          des: "All Natural Ingredients.",
          alt: "Psoriasis Cream",
        },
        {
          id: 3,
          image: "offers/offer-03.png",
          title: "Psoriasis Cream",
          des: "All Natural Ingredients.",
          alt: "Psoriasis Cream",
        },
        {
          id: 4,
          image: "offers/offer-03.png",
          title: "Psoriasis Cream",
          des: "All Natural Ingredients.",
          alt: "Psoriasis Cream",
        },
      ],
    };
  },
  methods: {
    getImgUrl: function (imagePath) {
      return require("@/assets/images/" + imagePath);
    },
  },
};
</script>
