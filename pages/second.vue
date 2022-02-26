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
              @click="toggle_Product(item)"
            >
              <template v-if="item.isAdd">Add to Cart</template>
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
                <div class="number-of-orders">
                  {{ item.count }}
                </div>
                <div class="card-info">
                  <div>
                    {{ item.name }}
                  </div>
                  <div class="card-info-price">${{ item.price }}</div>

                  <div class="amount-of-orders">
                    <div @click="remove_Product(item.id)" class="minus-img">
                      <img src="./../assets/images/second/chevron.svg" />
                    </div>
                    {{ item.count }}
                    <div @click="raise_Product(item.id)" class="plus-img">
                      <img src="./../assets/images/second/chevron.svg" />
                    </div>
                    <div class="amount-of-orders-price">${{ cardsum }}</div>
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
          <div class="sum-container">$ {{ cardsum }}</div>
        </div>
        <div class="sum-layout">
          Tax:
          <div class="sum-container">$ {{ tax }}</div>
        </div>
        <div class="sum-layout">
          Total:
          <div class="sum-container">$ {{ total }}</div>
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

      card: [],
    };
  },

  computed: {
    cardsum() {
      let sum = 0;
      this.card.forEach(function (product) {
        sum += product.price * product.count;
      });
      return sum.toFixed(2);
    },
    tax() {
      let tax = this.cardsum * 0.0975;
      return tax.toFixed(2);
    },
    total() {
      let total = this.cardsum * 1 + this.tax * 1;
      return total.toFixed(2);
    },
  },

  methods: {
    toggle_Product: function (product) {
      const index = this.card.findIndex(function (element) {
        return element.id === product.id;
      });
      if (index === -1) {
        this.card.push({ ...product });
        product.isAdd = false;
      } else {
        this.card.splice(index, 1);
        product.isAdd = true;
      }
    },

    raise_Product: function (productId) {
      const product = this.card.find(function (element) {
        return element.id === productId;
      });
      product.count += 1;
    },
    remove_Product: function (productId) {
      const product = this.card.find(function (element) {
        return element.id === productId;
      });
      const index = this.card.findIndex(function (element) {
        return element.id === productId;
      });
      if (product.count > 1) {
        product.count -= 1;
      } else {
        this.card.splice(index, 1);
      }
    },
  },
};
</script>

<style scoped lang="scss">
@import "./../assets/styles/second.scss";
</style>