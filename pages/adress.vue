<template>
  <section class="common-section">
    <div class="container">
      <div class="row">
        <div class="col-md-3">
          <Theslidebar />
        </div>
        <div class="col-md-9">
          <h1 class="section-title">Adress</h1>
          <div class="row">
            <div class="col-md-6" v-for="(item, index) in items" :key="item.id">
            <div>
              <div class="data-box">
                <div class="box-content">
                <h5>Home</h5>
                <p>01063987432</p>
                <p>26/C Mohammadpur Dhaka, Bangladesh</p>
                <a href="#">Edit</a>
              </div>
              </div>
              <button v-on:click.prevent="removeItem(index)" class="btn-delete">
                <i class="far fa-trash-alt"></i>
              </button>
            </div>
          </div>

          
          </div>
          <button @click="addItem" class="btn-great">
            <div class="btn-inner">
              <p>
                <i class="fas fa-plus"></i>              </p>
              <span>Add New Delivery Address</span>
            </div>
          </button>
         
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Theslidebar from "../components/TheSidebar.vue";
export default {
  name: "AdressPage",
  layout: "main",
  components: {
    Theslidebar,
  },
  data() {
    return {
      items: [],
    };
  },
  methods: {
    addItem() {
      this.items.push("");
    },
    removeItem(index) {
      this.items.splice(index, 1);
    },
  },
};
</script>
