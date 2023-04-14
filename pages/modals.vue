<template>
  <section class="common-section">
    <div class="container">
      <button
        type="button"
        class="btn-main"
        data-toggle="modal"
        data-target="#modal-1"
      >
        moadal#1
      </button>
      <button
        type="button"
        class="btn-main"
        data-toggle="modal"
        data-target="#modal-2"
      >
        moadal#2
      </button>
      <button
        type="button"
        class="btn-main"
        data-toggle="modal"
        data-target="#modal-3 "
      >
        moadal#3
      </button>
      <button
        type="button"
        class="btn-main"
        data-toggle="modal"
        data-target="#modal-4 "
      >
        moadal#4
      </button>
      <button
        type="button"
        class="btn-main"
        data-toggle="modal"
        data-target="#modal-5 "
      >
        moadal#5
      </button>
      <button
        type="button"
        class="btn-main"
        data-toggle="modal"
        data-target="#modal-6 "
      >
        moadal#6
      </button>
      <button
        type="button"
        class="btn-main"
        data-toggle="modal"
        data-target="#modal-7 "
      >
        moadal#7
      </button>
      <button
        type="button"
        class="btn-main"
        data-toggle="modal"
        data-target="#modal-8 "
      >
        moadal#8
      </button>

      <!-- Modal -->
      <div class="modal fade" id="modal-1" aria-hidden="true">
        <div class="modal-dialog" role="document">
          <div class="modal-content">
            <h5 class="modal-title">Add Payment Method</h5>
            <button
              type="button"
              class="close"
              data-dismiss="modal"
              aria-label="Close"
            >
              <span aria-hidden="true"
                ><i class="fa fa-times" aria-hidden="true"></i>
              </span>
            </button>

            <div class="modal-body">
              <form action="">
                <div class="form-group">
                  <select class="form-control">
                    <option selected>Type</option>
                    <option value="1">One</option>
                    <option value="2">Two</option>
                    <option value="3">Three</option>
                  </select>
                </div>
                <div class="form-group">
                  <input
                    class="form-control"
                    type="text"
                    placeholder="Card Name"
                  />
                </div>
                <div class="form-group">
                  <input
                    class="form-control"
                    type="text"
                    placeholder="Card Number"
                  />
                </div>
                <div class="form-group">
                  <input
                    class="form-control"
                    type="text"
                    placeholder="Expiration Date"
                  />
                </div>
                <div class="form-group">
                  <input class="form-control" type="text" placeholder="cvv" />
                </div>

                <div class="modal-footer">
                  <button type="submit" class="btn-main btn-block">Add</button>
                </div>
              </form>
            </div>
          </div>
        </div>
      </div>
      <div
        class="modal fade"
        id="modal-2"
        tabindex="-1"
        role="dialog"
        aria-hidden="true"
      >
        <div class="modal-dialog" role="document">
          <div class="modal-content">
            <h5 class="modal-title">Add New List</h5>
            <button
              type="button"
              class="close"
              data-dismiss="modal"
              aria-label="Close"
            >
              <span aria-hidden="true"
                ><i class="fa fa-times" aria-hidden="true"></i>
              </span>
            </button>

            <div class="modal-body">
              <div class="form-group">
                <input class="form-control" type="text" placeholder="Name" />
              </div>
            </div>
            <div class="modal-footer">
              <button type="button" class="btn-main btn-block">Add</button>
            </div>
          </div>
        </div>
      </div>
      <div class="modal fade" id="modal-3" aria-hidden="true">
        <div class="modal-dialog" role="document">
          <div class="modal-content">
            <button
              type="button"
              class="close"
              data-dismiss="modal"
              aria-label="Close"
            >
              <span aria-hidden="true"
                ><i class="fa fa-times" aria-hidden="true"></i>
              </span>
            </button>

            <div class="modal-body">
              <h3>Log Out?</h3>
              <p>Are you Sure Want to log out?</p>
            </div>
            <div class="modal-footer">
          
              
              <button
                type="button"
                class="btn-main btn-md btn-close"
                data-dismiss="modal"
              >
                Cancel
              </button>

              <button type="button" class="btn-main btn-md">Logout</button>
            </div>
          </div>
        </div>
      </div>
      <div class="modal fade" id="modal-4" aria-hidden="true">
        <div class="modal-dialog" role="document">
          <div class="modal-content">
            <h5 class="modal-title">Change Password</h5>
            <button
              type="button"
              class="close"
              data-dismiss="modal"
              aria-label="Close"
            >
              <span aria-hidden="true"
                ><i class="fa fa-times" aria-hidden="true"></i>
              </span>
            </button>

            <div class="modal-body">
              <form action="">
                <div class="form-group">
                  <input
                    class="form-control"
                    type="text"
                    placeholder="Current Password"
                  />
                  <a href="#">
                    <img
                      class="password-show"
                      src="~/assets/images/pass-show.svg"
                      alt=""
                  /></a>
                </div>
                <div class="form-group">
                  <input
                    class="form-control"
                    type="text"
                    placeholder="New Password"
                  />
                  <a href="#">
                    <img
                      class="password-show"
                      src="~/assets/images/pass-show.svg"
                      alt=""
                  /></a>
                </div>
                <div class="form-group">
                  <input
                    class="form-control"
                    type="text"
                    placeholder="ReType Password"
                  />
                  <a href="#"
                    ><img
                      class="password-hide"
                      src="~/assets/images/pass-hide.svg"
                      alt=""
                  /></a>
                </div>
              </form>
            </div>
            <div class="modal-footer">
              <button type="button" class="btn-main btn-block">Change</button>
            </div>
          </div>
        </div>
      </div>
      <div class="modal fade" id="modal-5" aria-hidden="true">
        <div class="modal-dialog" role="document">
          <div class="modal-content">
            <h5 class="modal-title">Add New Adress</h5>
            <button
              type="button"
              class="close"
              data-dismiss="modal"
              aria-label="Close"
            >
              <span aria-hidden="true"
                ><i class="fa fa-times" aria-hidden="true"></i>
              </span>
            </button>

            <div class="modal-body">
              <form action="">
                <div class="form-group">
                  <input class="form-control" type="text" placeholder="Name" />
                </div>
                <div class="form-group">
                  <input
                    class="form-control"
                    type="text"
                    placeholder="Phone Number"
                  />
                </div>
                <div class="form-group">
                  <select class="form-control">
                    <option selected>Governorate</option>
                    <option value="1">One</option>
                    <option value="2">Two</option>
                    <option value="3">Three</option>
                  </select>
                </div>
                <div class="form-group">
                  <select class="form-control">
                    <option selected>City</option>
                    <option value="1">One</option>
                    <option value="2">Two</option>
                    <option value="3">Three</option>
                  </select>
                </div>

                <div class="form-group">
                  <input
                    class="form-control"
                    type="text"
                    placeholder="Location"
                  />
                </div>
                <div class="form-group">
                  <input
                    class="form-control"
                    type="text"
                    placeholder="Zip Code"
                  />
                </div>
                <div class="custom-control custom-checkbox">
                  <input
                    type="checkbox"
                    class="custom-control-input"
                    id="customCheck1"
                  />
                  <label class="custom-control-label" for="customCheck1"
                    >Make Default Shipping Address</label
                  >
                </div>
                <div class="modal-footer">
                  <button type="submit" class="btn-main btn-block">Add</button>
                </div>
              </form>
            </div>
          </div>
        </div>
      </div>
      <div
        class="modal fade"
        id="modal-6"
        tabindex="-1"
        role="dialog"
        aria-hidden="true"
      >
        <div class="modal-dialog modal-xl" role="document">
          <div class="modal-content">
            <h5 class="modal-title">Order #65478913</h5>
            <button
              type="button"
              class="close"
              data-dismiss="modal"
              aria-label="Close"
            >
              <span aria-hidden="true"
                ><i class="fa fa-times" aria-hidden="true"></i>
              </span>
            </button>

            <div class="modal-body">
              <div class="row">
                <div class="col-md-7">
                  <div class="cart-body">
                    <h5>Product</h5>
                    <div class="product-cart">
                      <div class="product-image">
                        <img src="~/assets/images/product-image.png" alt="" />
                      </div>
                      <div class="product-name">
                        <p>Psoriasis Cream<span class="ml-3">1 KG</span></p>
                        <span class="cost">11.99 KWD</span>
                      </div>
                      <div class="product-weight">
                        <p>3 KG</p>
                      </div>
                      <div class="product-price">
                        <p class="price-color">35.97 KWD</p>
                      </div>
                    </div>
                    <div class="product-cart">
                      <div class="product-image">
                        <img src="~/assets/images/product-image.png" alt="" />
                      </div>
                      <div class="product-name">
                        <p>Psoriasis Cream<span class="ml-3">1 KG</span></p>
                        <span class="cost">11.99 KWD</span>
                      </div>
                      <div class="product-weight">
                        <p>3 KG</p>
                      </div>
                      <div class="product-price">
                        <p class="price-color">35.97 KWD</p>
                      </div>
                    </div>
                    <div class="product-cart">
                      <div class="product-image">
                        <img src="~/assets/images/product-image.png" alt="" />
                      </div>
                      <div class="product-name">
                        <p>Psoriasis Cream<span class="ml-3">1 KG</span></p>
                        <span class="cost">11.99 KWD</span>
                      </div>
                      <div class="product-weight">
                        <p>3 KG</p>
                      </div>
                      <div class="product-price">
                        <p class="price-color">35.97 KWD</p>
                      </div>
                    </div>
                    <div class="product-cart">
                      <div class="product-image">
                        <img src="~/assets/images/product-image.png" alt="" />
                      </div>
                      <div class="product-name">
                        <p>Psoriasis Cream<span class="ml-3">1 KG</span></p>
                        <span class="cost">11.99 KWD</span>
                      </div>
                      <div class="product-weight">
                        <p>3 KG</p>
                      </div>
                      <div class="product-price">
                        <p class="price-color">35.97 KWD</p>
                      </div>
                    </div>
                    <div class="product-cart">
                      <div class="product-image">
                        <img src="~/assets/images/product-image.png" alt="" />
                      </div>
                      <div class="product-name">
                        <p>Psoriasis Cream<span class="ml-3">1 KG</span></p>
                        <span class="cost">11.99 KWD</span>
                      </div>
                      <div class="product-weight">
                        <p>3 KG</p>
                      </div>
                      <div class="product-price">
                        <p class="price-color">35.97 KWD</p>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="col-md-5">
                  <div class="order-status">
                    <h5>Status</h5>
                    <div class="progress-line">
                      <div class="progress-rate"></div>
                      <div class="status">
                        <div class="dot completed"></div>
                      </div>
                      <div class="status">
                        <div class="dot completed"></div>
                      </div>
                      <div class="status">
                        <div class="dot completed"></div>
                      </div>
                      <div class="status">
                        <div class="dot completed"></div>
                      </div>
                      <div class="status">
                        <div class="dot completed"></div>
                      </div>
                    </div>
                    <span class="status-type">Shipped</span>
                  </div>
                  <div class="order-data">
                    <ul>
                      <h5>Adress</h5>
                      <li>11th Fareed Sebae St., Haram, Giza.</li>

                      <h5>Summary</h5>
                      <li>Total Items<span>8</span></li>
                      <li>Payment Type<span>Cash</span></li>
                      <li>Price<span>60 KWD</span></li>
                      <li>Shipping<span>10 KWD</span></li>
                      <li>Discount<span>10 KWD</span></li>
                      <li>
                        <div class="border-line"></div>
                      </li>
                      <li>Total Price<span>60 KWD</span></li>
                    </ul>
                  </div>

                  <button type="button" class="btn-main btn-block">
                    Cancel Order
                  </button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div
        class="modal fade"
        id="modal-7"
        tabindex="-1"
        role="dialog"
        aria-hidden="true"
      >
        <div class="modal-dialog modal-xl" role="document">
          <div class="modal-content">
            <h5 class="modal-title">Order #65478913</h5>
            <button
              type="button"
              class="close"
              data-dismiss="modal"
              aria-label="Close"
            >
              <span aria-hidden="true"
                ><i class="fa fa-times" aria-hidden="true"></i>
              </span>
            </button>

            <div class="modal-body">
              <div class="row">
                <div class="col-md-7">
                  <div class="cart-body">
                    <h5>Product</h5>
                    <div class="product-cart">
                      <div class="product-image">
                        <img src="~/assets/images/product-image.png" alt="" />
                      </div>
                      <div class="product-name">
                        <p>Psoriasis Cream<span class="ml-3">1 KG</span></p>
                        <span class="cost">11.99 KWD</span>
                      </div>
                      <div class="product-weight">
                        <p>3 KG</p>
                      </div>
                      <div class="product-price">
                        <p class="price-color">35.97 KWD</p>
                      </div>
                    </div>
                    <div class="product-cart">
                      <div class="product-image">
                        <img src="~/assets/images/product-image.png" alt="" />
                      </div>
                      <div class="product-name">
                        <p>Psoriasis Cream<span class="ml-3">1 KG</span></p>
                        <span class="cost">11.99 KWD</span>
                      </div>
                      <div class="product-weight">
                        <p>3 KG</p>
                      </div>
                      <div class="product-price">
                        <p class="price-color">35.97 KWD</p>
                      </div>
                    </div>
                    <div class="product-cart">
                      <div class="product-image">
                        <img src="~/assets/images/product-image.png" alt="" />
                      </div>
                      <div class="product-name">
                        <p>Psoriasis Cream<span class="ml-3">1 KG</span></p>
                        <span class="cost">11.99 KWD</span>
                      </div>
                      <div class="product-weight">
                        <p>3 KG</p>
                      </div>
                      <div class="product-price">
                        <p class="price-color">35.97 KWD</p>
                      </div>
                    </div>
                    <div class="product-cart">
                      <div class="product-image">
                        <img src="~/assets/images/product-image.png" alt="" />
                      </div>
                      <div class="product-name">
                        <p>Psoriasis Cream<span class="ml-3">1 KG</span></p>
                        <span class="cost">11.99 KWD</span>
                      </div>
                      <div class="product-weight">
                        <p>3 KG</p>
                      </div>
                      <div class="product-price">
                        <p class="price-color">35.97 KWD</p>
                      </div>
                    </div>
                    <div class="product-cart">
                      <div class="product-image">
                        <img src="~/assets/images/product-image.png" alt="" />
                      </div>
                      <div class="product-name">
                        <p>Psoriasis Cream<span class="ml-3">1 KG</span></p>
                        <span class="cost">11.99 KWD</span>
                      </div>
                      <div class="product-weight">
                        <p>3 KG</p>
                      </div>
                      <div class="product-price">
                        <p class="price-color">35.97 KWD</p>
                      </div>
                    </div>
                  </div>
                </div>
                <div class="col-md-5">
                  <div class="order-status confirmed">
                    <h5>Status</h5>
                    <div class="progress-line">
                      <div class="progress-rate"></div>
                      <div class="status">
                        <div class="dot completed"></div>
                      </div>
                      <div class="status">
                        <div class="dot"></div>
                      </div>
                      <div class="status">
                        <div class="dot"></div>
                      </div>
                      <div class="status">
                        <div class="dot"></div>
                      </div>
                      <div class="status">
                        <div class="dot"></div>
                      </div>
                    </div>
                    <span class="status-type">Confirmed</span>
                  </div>
                  <div class="order-data">
                    <ul>
                      <h5>Adress</h5>
                      <li>11th Fareed Sebae St., Haram, Giza.</li>

                      <h5>Summary</h5>
                      <li>Total Items<span>8</span></li>
                      <li>Payment Type<span>Cash</span></li>
                      <li>Price<span>60 KWD</span></li>
                      <li>Shipping<span>10 KWD</span></li>
                      <li>Discount<span>10 KWD</span></li>
                      <li>
                        <div class="border-line"></div>
                      </li>
                      <li>Total Price<span>60 KWD</span></li>
                    </ul>
                  </div>

                  <button type="button" class="btn-main btn-block">
                    Cancel Order
                  </button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div
        class="modal fade"
        id="modal-8"
        tabindex="-1"
        role="dialog"
        aria-hidden="true"
      >
        <div class="modal-dialog" role="document">
          <div class="modal-content">
            <div class="modal-body text-center">
              <img src="~/assets/images/modal-image.png" alt="" />
              <h5>Psoriasis Cream<span>1 KG</span></h5>
              <p class="attention-massage">
                Sorry, there is a maximum limit for this product per user.
              </p>
            </div>
            <button type="button" class="btn-main btn-block">Ok</button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
  
  <script>
export default {
  name: "modalsPage",
  layout: "main",
};
</script>
  