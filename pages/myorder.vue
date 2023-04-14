<template>
  <section class="common-section">
    <div class="container">
      <div class="row">
        <div class="col-md-3">
          <Theslidebar />
        </div>
        <div class="col-md-9">
          <h1 class="section-title">My Order</h1>

          <div class="table-responsive-md">
            <table class="table order-table">
              <tbody>
                <tr>
                  <th scope="row">#65478913</th>
                  <td>15 / 11 / 2021</td>
                  <td>11.99 KWD</td>
                  <td class="black-color">2</td>
                  <td class="order-confirmed">Confirmed</td>
                </tr>
                <tr>
                  <th scope="row">#65478913</th>
                  <td>15 / 11 / 2021</td>
                  <td>11.99 KWD</td>
                  <td class="black-color">2</td>
                  <td class="order-delivery">Delivery</td>
                </tr>
                <tr>
                  <th scope="row">#65478913</th>
                  <td>15 / 11 / 2021</td>
                  <td>11.99 KWD</td>
                  <td class="black-color">2</td>
                  <td class="order-Shipped">Shipped</td>
                </tr>
                <tr>
                  <th scope="row">#65478913</th>
                  <td>15 / 11 / 2021</td>
                  <td>11.99 KWD</td>
                  <td class="black-color">2</td>
                  <td class="order-delivery">Delivery</td>
                </tr>
                <tr>
                  <th scope="row">#65478913</th>
                  <td>15 / 11 / 2021</td>
                  <td>11.99 KWD</td>
                  <td class="black-color">2</td>
                  <td class="order-cancel">Cancel</td>
                </tr>
                <tr>
                  <th scope="row">#65478913</th>
                  <td>15 / 11 / 2021</td>
                  <td>11.99 KWD</td>
                  <td class="black-color">2</td>
                  <td class="order-confirmed">Processing</td>
                </tr>
              </tbody>
            </table>
          </div>
          <ThePagnation />
         
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import Theslidebar from "../components/TheSidebar.vue";
import ThePagnation from "../components/ThePagnation.vue";
export default {
  name: "MyOrderPage",
  layout: "main",
  components: {
    Theslidebar,
    ThePagnation,
  },
};
</script>
