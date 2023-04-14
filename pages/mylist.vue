<template>
  <section class="common-section">
    <div class="container">
      <div class="row">
        <div class="col-md-3">
          <Theslidebar />
        </div>
        <div class="col-md-9">
          <h1 class="section-title">My List</h1>
          <div class="row">
            <div class="col-md-6" v-for="(item, index) in items" :key=item.id>
              <div>
                <div class="data-box">
                  <div class="box-content">
                    <h5>My List 1</h5>
                    <p>3 Items</p>
                    <a href="#">Change Name</a>
                  </div>
                </div>
                <button
                  v-on:click.prevent="removeItem(index)"
                  class="btn-delete"
                >
                  <i class="far fa-trash-alt"></i>
                </button>
              </div>
            </div>
          </div>
          <button @click="addItem" class="btn-great">
            <div class="btn-inner">
              <p>
                <i class="fa fa-plus"></i>
              </p>
              <span> Create a new list</span>
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
  name: "MyListPage",
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
