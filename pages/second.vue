<template>
  <div class="second">
    <div class="background">
      <img class="bg-left" src="./../assets/images/second/bg__left.svg" />
      <img
        class="bg-top-right"
        src="./../assets/images/second/bg__top-right.svg"
      />
      <img
        class="bg-btm-right"
        src="./../assets/images/second/bg__btm-right.svg"
      />
    </div>
    <div class="menu">
      <div>
        <h1 class="to-go-menu menu-item">To Go Menu</h1>
        <div
          class="menu-item"
          v-for="item in menu"
          :key="item.id"
          :style="{
            'background-color': item.color,
          }"
        >
          <img class="menu-img" :src="item.img" />
          <div class="menu-item-info">
            <div class="menu-title">{{ item.name }}</div>
            <div class="price">${{ item.price }}</div>
            <div 
              class="btn-bay" 
              id="btnFrenchFries" 
              @click="addProduct(item)"
            >
              <template v-if="item.isAdd"> Add to Cart </template>
              <template v-else>
                <img
                  class="img-check"
                  src="./../assets/images/second/check.svg"
                />
                In Cart
              </template>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="card">
      <div class="your-card">Your Card</div>
      <div class="card-content">
        <div class="card-item">
            <div 
                v-for="item in card" 
                :key="item.id"
            >
              <template>
                <div class="card-item-tamplate">
                  <img class="card-img" :src="item.img" />
                  <div class="numberOfOrders">
                    {{ item.count }}
                  </div>
                  <div class="card-info">
                    <div>
                      {{ item.name }}
                    </div>
                    <div class="card-info-price">${{item.price}}</div>

                    <div class="amount-of-orders">
                      <div @click="removeProduct(item.id)" class="minus-img">
                        <img src="./../assets/images/second/chevron.svg" />
                      </div>
                      {{ item.count }}
                      <div @click="raiseProduct(item.id)" class="plus-img">
                        <img src="./../assets/images/second/chevron.svg" />
                      </div>
                      <div class="amount-of-orders-price">
                        ${{item.price * item.count}}
                      </div>
                    </div>
                  </div>
                </div>
                <div class="card-line-tamplate"></div>
              </template>
          </div>
        </div>
        <div class="card-line"></div>
      </div>
      <div class="sum">
        <div class="sum-layout">
          Subtotal:
          <div class="sum-container">$ {{ subtotal }}</div>
        </div>
        <div class="sum-layout">
          Tax:
          <div class="sum-container">
            $ {{ Math.floor(subtotal * 0.0975 * 100) / 100 }}
          </div>
        </div>
        <div class="sum-layout">
          Total:
          <div class="sum-container">
            $ {{ Math.floor((subtotal + subtotal * 0.0975) * 100) / 100 }}
          </div>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
export default {
  colorMode: "second",
  data: function () {
    return {
      menu: [
        {
          id: 1,
          name: "French Fries with Ketchup",
          price: 2.23,
          count: 1,
          img: "/images/second/plate__french-fries.png",
          color: "#e1f1fe",
          isAdd: true,
        },
        {
          id: 2,
          name: "Salmon and Vegetables",
          price: 5.12,
          count: 1,
          img: "/images/second/plate__salmon-vegetables.png",
          color: "#ffe2f0",
          isAdd: true,
        },
        {
          id: 3,
          name: "Spaghetti with Meat Sauce",
          price: 7.82,
          count: 1,
          img: "/images/second/plate__spaghetti-meat-sauce.png",
          color: "#f7f7fe",
          isAdd: true,
        },
        {
          id: 4,
          name: "Chicken Salad with Parmesean",
          price: 6.98,
          count: 1,
          img: "/images/second/plate__chicken-salad.png",
          color: "#defef0",
          isAdd: true,
        },
        {
          id: 5,
          name: "Fish Sticks and Fries",
          price: 6.34,
          count: 1,
          img: "/images/second/plate__fish-sticks-fries.png",
          color: "#e1f1fe",
          isAdd: true,
        },
        {
          id: 6,
          name: "Ravioli",
          price: 6.45,
          count: 1,
          img: "/images/second/plate__ravioli.png",
          color: "#ffe2f0",
          isAdd: true,
        },
        {
          id: 7,
          name: "Tortellini",
          price: 6.05,
          count: 1,
          img: "/images/second/plate.png",
          color: "#f7f7fe",
          isAdd: true,
        },
        {
          id: 8,
          name: "Bacon, Eggs, and Toast",
          price: 5.99,
          count: 1,
          img: "/images/second/plate__bacon-eggs.png",
          color: "#defef0",
          isAdd: true,
        },
      ],

      subtotal: 10,

      card: [],

    };
  },
  methods: {
    addProduct: function (product) {
      var index = this.card.indexOf(product);
      if (index > -1) {
          this.card.splice(index, 1);
      }else{
        this.card.push(product);
        this.subtotal = this.subtotal + this.card.price;
      }        
    },

    raiseProduct: function (sum) {
      this.card.count = this.card.count + 1;
      this.subtotal =
        Math.floor((this.subtotal * this.card.count * this.card.price) * 100) / 100;
    },
    removeProduct: function (sum) {
      if (this.numberOfFrenchFries > 1) {
        this.numberOfFrenchFries = this.numberOfFrenchFries - 1;
        this.totalFrenchFries =
          Math.floor((this.totalFrenchFries - this.priceFrenchFries) * 100) /
          100;
        this.subtotal =
          Math.floor((this.subtotal - this.priceFrenchFries) * 100) / 100;
      } else if (this.numberOfFrenchFries === 1) {
        this.isAddFrenchFries = true;
        var element = document.getElementById("btnFrenchFries");
        element.style.backgroundColor = "#6B00F5";
        this.subtotal =
          Math.floor((this.subtotal - this.priceFrenchFries) * 100) / 100;
      }
    },
  }
};
</script>

<style scoped lang="scss">
@import "./../assets/styles/second.scss";
</style>