<template>
  <section class="offer-section">
    <div class="container">
      <h1 class="section-title">Offers</h1>

      <div class="row">
        <div class="col-lg-3 col-md-4 col-sm-6">
          <div class="item-box">
            <div class="image-item">
              <!-- <a
                class="add-fav"
                :class="{ 'like': offer.favourite, 'dislike': !offer.favourite }"
                @click="FavToggle(offer)"
              >
            </a> -->

              <img
                src="~/assets/images/offers/offer-01.png"
                alt="Psoriasis Cream"
              />
            </div>
            <div class="item-details">
              <h4>Psoriasis Cream</h4>
              <p>All Natural Ingredients.</p>
              <p class="new-price">$10.99</p>
              <del class="old-price">$24.99</del>
            </div>

            <div class="item-add">
              <button class="value-button decrease-button" @click="count--">
                <i class="fa fa-minus" aria-hidden="true"></i>
              </button>
              <div class="items-number">{{ count }}</div>
              <button class="value-button increase-button" @click="count++">
                <i class="fa fa-plus" aria-hidden="true"></i>
              </button>
            </div>
          </div>
        </div>

        <div
          class="col-lg-3 col-md-4 col-sm-6"
          v-for="offer in offers"
          :key="offer.id"
        >
          <div class="item-box">
            <div class="image-item">
              <a
                class="add-fav"
                :class="{ 'like': offer.favourite, 'dislike': !offer.favourite }"
                @click="FavToggle(offer)"
              >
            </a>
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
  </section>
</template>
<script>
export default {
  name: "TheOffers",
  layout: "component",
  data() {
    return {
      count: 0,
      favourite: false,
      offers: [
        {
          id: 1,
          image: "offers/offer-02.png",
          title: "Psoriasis Cream",
          src: require("~/assets/images/like.png"),
          des: "All Natural Ingredients.",
          alt: "Psoriasis Cream",
          favourite: false,
        },
        {
          id: 2,
          image: "offers/offer-03.png",
          title: "Psoriasis Cream",
          des: "All Natural Ingredients.",
          alt: "Psoriasis Cream",
          favourite: false,
        },
        {
          id: 3,
          image: "offers/offer-03.png",
          title: "Psoriasis Cream",
          des: "All Natural Ingredients.",
          alt: "Psoriasis Cream",
          favourite: false,
        },
        {
          id: 4,
          image: "offers/offer-03.png",
          title: "Psoriasis Cream",
          des: "All Natural Ingredients.",
          alt: "Psoriasis Cream",
          favourite: false,
        },
        {
          id: 5,
          image: "offers/offer-01.png",
          title: "Psoriasis Cream",
          des: "All Natural Ingredients.",
          alt: "Psoriasis Cream",
          favourite: false,
        },
        {
          id: 6,
          image: "offers/offer-03.png",
          title: "Psoriasis Cream",
          des: "All Natural Ingredients.",
          alt: "Psoriasis Cream",
          favourite: false,
        },
        {
          id: 7,
          image: "offers/offer-02.png",
          title: "Psoriasis Cream",
          des: "All Natural Ingredients.",
          alt: "Psoriasis Cream",
          favourite: false,
        },
      ],
    };
  },

  methods: {
    getImgUrl: function (imagePath) {
      return require("@/assets/images/" + imagePath);
    },

    FavToggle(offer) {
      return (offer.favourite = !offer.favourite);
    },
  },
};
</script>
<style scoped>
.like {
  background-image: url("~/assets/images/like.png");
}
.dislike {
  background-image: url("~/assets/images/dislike.png");
}
</style>
