<template>
    <div class="second">
        <div class="menu">
            <div>
                <h1 class="to-go-menu menu-item">
                    To Go Menu
                </h1>
                <div
                    class="menu-item pattens-blue"
                >
                    <img class="menu-img" src="./../assets/images/second/plate__french-fries.png"/>
                    <div class="menu-item-info">
                        <div
                            class="menu-title"
                        >
                            French Fries with Ketchup
                        </div>
                        <div 
                            class="price"
                        >
                            ${{priceFrenchFries}}
                        </div>
                        <div
                            class="btn-bay"
                            id="btnFrenchFries"
                            @click="addFrenchFries"
                        >
                            <template v-if="isAddFrenchFries">
                                Add to Cart
                            </template>
                            <template v-else >
                                <div
                                >                                    
                                </div>
                                    <img class="img-check" src="./../assets/images/second/check.svg" />
                                    In Cart
                            </template>
                        </div>
                    </div>
                </div>
                <div 
                    class="menu-item pale-rose">
                    <img class="menu-img" src="./../assets/images/second/plate__salmon-vegetables.png" />
                    <div class="menu-item-info">
                        <div
                            class="menu-title"
                        >
                            Salmon and Vegetables
                        </div>
                        <div 
                            class="price"
                        >
                            ${{priceSalmonAndVegetables}}
                        </div>
                        <div
                            class="btn-bay"
                            id="btnSalmonAndVegetables"
                            @click="addSalmonAndVegetables"
                        >
                            <template v-if="isAddSalmonAndVegetables">
                                Add to Cart
                            </template>
                            <template v-else >
                                <div
                                >                                    
                                </div>
                                    <img class="img-check" src="./../assets/images/second/check.svg" />
                                    In Cart
                            </template>
                        </div>
                    </div>
                </div>
                <div
                    class="menu-item ghost-white"
                >
                    <img class="menu-img" src="./../assets/images/second/plate__spaghetti-meat-sauce.png" />
                    <div class="menu-item-info">
                        <div
                            class="menu-title"
                        >
                            Spaghetti with Meat Sauce
                        </div>
                        <div 
                            class="price"
                        >
                            ${{priceSpaghettiWithMeatSauce}}
                        </div>
                        <div
                            class="btn-bay"
                            id="btnSpaghettiWithMeatSauce"
                            @click="addSpaghettiWithMeatSauce"
                        >
                            <template v-if="isAddSpaghettiWithMeatSauce">
                                Add to Cart
                            </template>
                            <template v-else >
                                <div
                                >                                    
                                </div>
                                    <img class="img-check" src="./../assets/images/second/check.svg" />
                                    In Cart
                            </template>
                        </div>
                    </div>
                </div>
                <div
                    class="menu-item white-ice"
                >
                    <img class="menu-img" src="./../assets/images/second/plate__chicken-salad.png" />
                    <div class="menu-item-info">
                        <div
                            class="menu-title"
                        >
                            Chicken Salad with Parmesean
                        </div>
                        <div 
                            class="price"
                        >
                            ${{priceChickenSaladwithParmesean}}
                        </div>
                        <div
                            class="btn-bay"
                            id="btnChickenSaladwithParmesean"
                            @click="addChickenSaladwithParmesean"
                        >
                            <template v-if="isAddChickenSaladwithParmesean">
                                Add to Cart
                            </template>
                            <template v-else >
                                <div
                                >                                    
                                </div>
                                    <img class="img-check" src="./../assets/images/second/check.svg" />
                                    In Cart
                            </template>
                        </div>
                    </div>
                </div>
                <div
                    class="menu-item pattens-blue"
                >
                    <img class="menu-img" src="./../assets/images/second/plate__fish-sticks-fries.png" />
                    <div class="menu-item-info">
                        <div
                            class="menu-title"
                        >
                            Fish Sticks and Fries
                        </div>
                        <div 
                            class="price"
                        >
                            ${{priceFishSticksAndFries}}
                        </div>
                        <div
                            class="btn-bay"
                            id="btnFishSticksAndFries"
                            @click="addFishSticksAndFries"
                        >
                            <template v-if="isAddFishSticksAndFries">
                                Add to Cart
                            </template>
                            <template v-else >
                                <div
                                >                                    
                                </div>
                                    <img class="img-check" src="./../assets/images/second/check.svg" />
                                    In Cart
                            </template>
                        </div>
                    </div>
                </div>
                <div
                    class="menu-item pale-rose"
                >
                    <img class="menu-img" src="./../assets/images/second/plate__ravioli.png" />
                    <div class="menu-item-info">
                        <div
                            class="menu-title"
                        >
                            Ravioli
                        </div>
                        <div 
                            class="price"
                        >
                            ${{priceRavioli}}
                        </div>
                        <div
                            class="btn-bay"
                            id="btnRavioli"
                            @click="addRavioli"
                        >
                            <template v-if="isAddRavioli">
                                Add to Cart
                            </template>
                            <template v-else >
                                <div
                                >                                    
                                </div>
                                    <img class="img-check" src="./../assets/images/second/check.svg" />
                                    In Cart
                            </template>
                        </div>
                    </div>
                </div>
                <div
                    class="menu-item ghost-white"
                >
                    <img class="menu-img" src="./../assets/images/second/plate.png" />
                    <div class="menu-item-info">
                        <div
                            class="menu-title"
                        >
                            Tortellini
                        </div>
                        <div 
                            class="price"
                        >
                            ${{priceTortellini}}
                        </div>
                        <div
                            class="btn-bay"
                            id="btnTortellini"
                            @click="addTortellini"
                        >
                            <template v-if="isAddTortellini">
                                Add to Cart
                            </template>
                            <template v-else >
                                <div
                                >                                    
                                </div>
                                    <img class="img-check" src="./../assets/images/second/check.svg" />
                                    In Cart
                            </template>
                        </div>
                    </div>
                </div>
                <div
                    class="menu-item white-ice"
                >
                    <img class="menu-img" src="./../assets/images/second/plate__bacon-eggs.png" />
                    <div class="menu-item-info">
                        <div
                            class="menu-title"
                        >
                            Bacon, Eggs, and Toast
                        </div>
                        <div 
                            class="price"
                        >
                            ${{priceBaconEggsAndToast}}
                        </div>
                        <div
                            class="btn-bay"
                            id="btnBaconEggsAndToast"
                            @click="addBaconEggsAndToast"
                        >
                            <template v-if="isAddBaconEggsAndToast">
                                Add to Cart
                            </template>
                            <template v-else >
                                <div
                                >                                    
                                </div>
                                    <img class="img-check" src="./../assets/images/second/check.svg" />
                                    In Cart
                            </template>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <div class="card">
            <div class="your-card">
                Your Card
            </div>
            <div class="card-content">
                <div
                    class="card-item"
                >
                    <template v-if="!isAddFrenchFries">
                        <div class="card-item-tamplate">
                            <img class="card-img" src="./../assets/images/second/plate__french-fries.png"/>
                            <div class="numberOfOrders">
                                {{numberOfFrenchFries}}
                            </div>
                            <div class="card-info">
                                <div>
                                    Fish Sticks and Fries
                                </div>
                                <div class="card-info-price">${{priceFrenchFries}}</div>
                            
                                <div class="amount-of-orders">
                                    <div 
                                        @click="removeFrenchFriesNumber"
                                        class="minus-img"
                                    > 
                                        <img src="./../assets/images/second/chevron.svg"/>
                                    </div>
                                        {{numberOfFrenchFries}}
                                    <div 
                                        @click="addFrenchFriesNumber"
                                        class="plus-img"
                                    >
                                        <img src="./../assets/images/second/chevron.svg"/>
                                    </div>
                                    <div class="amount-of-orders-price">
                                        ${{totalPriceFrenchFries}}
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="card-line-tamplate"></div>
                    </template>
                    <template v-if="!isAddFrenchFries">
                        <div class="card-item-tamplate">
                            <img class="card-img" src="./../assets/images/second/plate__french-fries.png"/>
                            <div class="numberOfOrders">
                                {{numberOfFrenchFries}}
                            </div>
                            <div class="card-info">
                                <div>
                                    Fish Sticks and Fries
                                </div>
                                <div class="card-info-price">${{priceFrenchFries}}</div>
                            
                                <div class="amount-of-orders">
                                    <div 
                                        @click="removeFrenchFriesNumber"
                                        class="minus-img"
                                    > 
                                        <img src="./../assets/images/second/chevron.svg"/>
                                    </div>
                                        {{numberOfFrenchFries}}
                                    <div 
                                        @click="addFrenchFriesNumber"
                                        class="plus-img"
                                    >
                                        <img src="./../assets/images/second/chevron.svg"/>
                                    </div>
                                    <div class="amount-of-orders-price">
                                        ${{totalPriceFrenchFries}}
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="card-line-tamplate"></div>
                    </template>
                    <template v-if="!isAddFrenchFries">
                        <div class="card-item-tamplate">
                            <img class="card-img" src="./../assets/images/second/plate__french-fries.png"/>
                            <div class="numberOfOrders">
                                {{numberOfFrenchFries}}
                            </div>
                            <div class="card-info">
                                <div>
                                    Fish Sticks and Fries
                                </div>
                                <div class="card-info-price">${{priceFrenchFries}}</div>
                            
                                <div class="amount-of-orders">
                                    <div 
                                        @click="removeFrenchFriesNumber"
                                        class="minus-img"
                                    > 
                                        <img src="./../assets/images/second/chevron.svg"/>
                                    </div>
                                        {{numberOfFrenchFries}}
                                    <div 
                                        @click="addFrenchFriesNumber"
                                        class="plus-img"
                                    >
                                        <img src="./../assets/images/second/chevron.svg"/>
                                    </div>
                                    <div class="amount-of-orders-price">
                                        ${{totalPriceFrenchFries}}
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="card-line-tamplate"></div>
                    </template>
                    <template v-if="!isAddFrenchFries">
                        <div class="card-item-tamplate">
                            <img class="card-img" src="./../assets/images/second/plate__french-fries.png"/>
                            <div class="numberOfOrders">
                                {{numberOfFrenchFries}}
                            </div>
                            <div class="card-info">
                                <div>
                                    Fish Sticks and Fries
                                </div>
                                <div class="card-info-price">${{priceFrenchFries}}</div>
                            
                                <div class="amount-of-orders">
                                    <div 
                                        @click="removeFrenchFriesNumber"
                                        class="minus-img"
                                    > 
                                        <img src="./../assets/images/second/chevron.svg"/>
                                    </div>
                                        {{numberOfFrenchFries}}
                                    <div 
                                        @click="addFrenchFriesNumber"
                                        class="plus-img"
                                    >
                                        <img src="./../assets/images/second/chevron.svg"/>
                                    </div>
                                    <div class="amount-of-orders-price">
                                        ${{totalPriceFrenchFries}}
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="card-line-tamplate"></div>
                    </template>
                </div>

                <div class="card-line"></div>
            </div>
                
            <div class="sum">
                <div class="sum-layout">
                    Subtotal:
                    <div class="sum-container">
                        $ {{subtotal}}
                    </div>
                </div>
                <div class="sum-layout">
                    Tax:
                    <div class="sum-container">
                        $ {{Math.floor((subtotal * 0.0975)* 100) / 100}}
                    </div>
                </div>
                <div class="sum-layout">
                    Total:
                    <div class="sum-container">
                        $ {{Math.floor((subtotal + (subtotal * 0.0975))* 100) / 100 }}
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
        totalPriceFrenchFries: 2.23,
        numberOfFrenchFries: 1,
        subtotal: 0,
        priceFrenchFries: 2.23,
        priceSalmonAndVegetables: 5.12,
        priceSpaghettiWithMeatSauce: 7.82,
        priceChickenSaladwithParmesean: 6.98,
        priceFishSticksAndFries:6.34,
        priceRavioli: 6.45,
        priceTortellini: 6.05,
        priceBaconEggsAndToast: 5.99,
        isAddFrenchFries: true,
        isAddSalmonAndVegetables: true,
        isAddSpaghettiWithMeatSauce: true,
        isAddChickenSaladwithParmesean: true,
        isAddFishSticksAndFries: true,
        isAddRavioli:true,
        isAddTortellini:true,
        isAddBaconEggsAndToast: true,
        orderPrice: 0
    }
  },
  methods:{
    addFrenchFries: function(){
        this.isAddFrenchFries = !this.isAddFrenchFries
        if (this.isAddFrenchFries === false){
            var element = document.getElementById("btnFrenchFries");
            element.style.backgroundColor = "black";
            this.orderPrice = this.orderPrice + this.priceFrenchFries;
        }else if (this.isAddFrenchFries === true){
            var element = document.getElementById("btnFrenchFries");
            element.style.backgroundColor = "#6B00F5";
            this.orderPrice = 0;
        }
        this.subtotal = this.orderPrice
    },
    addSalmonAndVegetables: function(){
        this.isAddSalmonAndVegetables = !this.isAddSalmonAndVegetables
        if (this.isAddSalmonAndVegetables === true){
            var element = document.getElementById("btnSalmonAndVegetables");
            element.style.backgroundColor = "#6B00F5";
            this.subtotal = this.subtotal - this.priceSalmonAndVegetables;
        }else if (this.isAddSalmonAndVegetables === false){
            var element = document.getElementById("btnSalmonAndVegetables");
            element.style.backgroundColor = "black";
            this.subtotal = this.subtotal + this.priceSalmonAndVegetables;
        }
    },
    addSpaghettiWithMeatSauce: function(){
        this.isAddSpaghettiWithMeatSauce = !this.isAddSpaghettiWithMeatSauce
        if (this.isAddSpaghettiWithMeatSauce === true){
            var element = document.getElementById("btnSpaghettiWithMeatSauce");
            element.style.backgroundColor = "#6B00F5";
            this.subtotal = this.subtotal - this.priceSpaghettiWithMeatSauce;
        }else if (this.isAddSpaghettiWithMeatSauce === false){
            var element = document.getElementById("btnSpaghettiWithMeatSauce");
            element.style.backgroundColor = "black";
            this.subtotal = this.subtotal + this.priceSpaghettiWithMeatSauce;
        }
    },
    addChickenSaladwithParmesean: function(){
        this.isAddChickenSaladwithParmesean = !this.isAddChickenSaladwithParmesean
        if (this.isAddChickenSaladwithParmesean === true){
            var element = document.getElementById("btnChickenSaladwithParmesean");
            element.style.backgroundColor = "#6B00F5";
            this.subtotal = this.subtotal - this.priceChickenSaladwithParmesean;
        }else if (this.isAddChickenSaladwithParmesean === false){
            var element = document.getElementById("btnChickenSaladwithParmesean");
            element.style.backgroundColor = "black";
            this.subtotal = this.subtotal + this.priceChickenSaladwithParmesean;
        }
    },
    addFishSticksAndFries: function(){
        this.isAddFishSticksAndFries = !this.isAddFishSticksAndFries
        if (this.isAddFishSticksAndFries === true){
            var element = document.getElementById("btnFishSticksAndFries");
            element.style.backgroundColor = "#6B00F5";
            this.subtotal = this.subtotal - this.priceFishSticksAndFries;
        }else if (this.isAddFishSticksAndFries === false){
            var element = document.getElementById("btnFishSticksAndFries");
            element.style.backgroundColor = "black";
            this.subtotal = this.subtotal + this.priceFishSticksAndFries;
        }
    },
    addRavioli: function(){
        this.isAddRavioli = !this.isAddRavioli
        if (this.isAddRavioli === true){
            var element = document.getElementById("btnRavioli");
            element.style.backgroundColor = "#6B00F5";
            this.subtotal = this.subtotal - this.priceRavioli;
        }else if (this.isAddRavioli === false){
            var element = document.getElementById("btnRavioli");
            element.style.backgroundColor = "black";
            this.subtotal = this.subtotal + this.priceRavioli;
        }
    },
    addTortellini: function(){
        this.isAddTortellini = !this.isAddTortellini
        if (this.isAddTortellini === true){
            var element = document.getElementById("btnTortellini");
            element.style.backgroundColor = "#6B00F5";
            this.subtotal = this.subtotal - this.priceTortellini;
        }else if (this.isAddTortellini === false){
            var element = document.getElementById("btnTortellini");
            element.style.backgroundColor = "black";
            this.subtotal = this.subtotal + this.priceTortellini;
        }
    },
    addBaconEggsAndToast: function(){
        this.isAddBaconEggsAndToast = !this.isAddBaconEggsAndToast
        if (this.isAddBaconEggsAndToast === true){
            var element = document.getElementById("btnBaconEggsAndToast");
            element.style.backgroundColor = "#6B00F5";
            this.subtotal = this.subtotal - this.priceBaconEggsAndToast;
        }else if (this.isAddBaconEggsAndToast === false){
            var element = document.getElementById("btnBaconEggsAndToast");
            element.style.backgroundColor = "black";
            this.subtotal = this.subtotal + this.priceBaconEggsAndToast;
        }
    },
    addFrenchFriesNumber: function() {
        this.numberOfFrenchFries = this.numberOfFrenchFries + 1
        this.totalPriceFrenchFries = this.totalPriceFrenchFries + this.priceFrenchFries
            this.subtotal = this.subtotal + this.priceFrenchFries;
    },
    removeFrenchFriesNumber: function() {
        if (this.numberOfFrenchFries > 1) {
            this.numberOfFrenchFries = this.numberOfFrenchFries - 1;
        this.totalPriceFrenchFries = this.totalPriceFrenchFries - this.priceFrenchFries
            this.subtotal = this.subtotal - this.priceFrenchFries;
        }else if (this.numberOfFrenchFries === 1){
            this.isAddFrenchFries = true
            var element = document.getElementById("btnFrenchFries");
            element.style.backgroundColor = "#6B00F5";
            this.subtotal = this.subtotal - this.priceFrenchFries;
            
        }
    },
  },
}
</script>


<style scoped lang="scss">
@import "./../assets/styles/second.scss";
</style>