<!-- <template>
  <section class="common-section bg-gray">
    <header class="section-header">
      <div class="container">
        <span>Our Work</span>
        <h2>Popular Works</h2>
      </div>
    </header>
    <div class="container">
     
      <div class="row">
        <div class="col-md-4" v-for="offer in offers" :key="offer.id">
          <div class="work-item js-tilt">
            <figure class="work-thumb">
              <img :src="getImgUrl(offer.image)" alt="Work 1" />
            </figure>
            <h5>{{ offer.title }}</h5>
          </div>
        </div>
      </div>
    </div>
    
  </section>
</template>

<script>
export default {
  data() {
    return {
      works: [
        {
          id: 0,
          image: "offers/offer-01.png",
          title: "Psoriasis Cream",
        },
        {
          id: 1,
          image: "offers/offer-02.png",
          title: "Psoriasis Cream",
        },
        {
          id: 2,
          image: "offers/offer-03.png",
          title: "Psoriasis Cream",
        },
        {
          id: 3,
          image: "offers/offer-04.png",
          title: "Psoriasis Cream",
        },
        {
          id: 4,
          image: "offers/offer-05.png",
          title: "Psoriasis Cream",
        },
        {
          id: 5,
          image: "offers/offer-07.png",
          title: "Psoriasis Cream",
        },
        {
          id: 5,
          image: "offers/offer-08.png",
          title: "Psoriasis Cream",
        },
        {
          id: 5,
          image: "offers/offer-06.png",
          title: "Psoriasis Cream",
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

<style></style> -->
