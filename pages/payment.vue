<template>
  <section class="common-section">
    <div class="container">
      <div class="row">
        <div class="col-md-3">
          <Theslidebar />
        </div>
        <div class="col-md-9">
          <h1 class="section-title">Payment Methods</h1>
          <div class="row">
          <div class="col-md-6" v-for="(item, index) in items" :key="item.id">
            <div>
              <div class="data-box">
                <div class="box-content">
                  <h5>Master Card</h5>
                  <p>**** **** **** 4986</p>
                  <p>Exp. 18 /5</p>
                  <a href="#">Edit</a>
                </div>
              </div>
              <button @:click.prevent="removeItem(index)" class="btn-delete">
                <i class="far fa-trash-alt"></i>
              </button>
            </div>
          </div>
        </div>

          <button @click="addItem" class="btn-great">
            <div class="btn-inner">
              <p>
                <i class="fas fa-credit-card"></i>
              </p>
              <span> Payment cards not found</span>
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
  name: "PaymentPage",
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
