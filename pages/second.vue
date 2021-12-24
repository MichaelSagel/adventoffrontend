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
                            ${{FrenchFries.price}}
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
                            ${{SalmonAndVegetables.price}}
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
                            ${{SpaghettiWithMeatSauce.price}}
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
                            ${{ChickenSaladwithParmesean.price}}
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
                            ${{FishSticksAndFries.price}}
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
                            ${{Ravioli.price}}
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
                            ${{Tortellini.price}}
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
                            ${{BaconEggsAndToast.price}}
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
                                <div class="card-info-price">${{FrenchFries.price}}</div>
                            
                                <div class="amount-of-orders">
                                    <div 
                                        @click="removeFrenchFries"
                                        class="minus-img"
                                    > 
                                        <img src="./../assets/images/second/chevron.svg"/>
                                    </div>
                                        {{numberOfFrenchFries}}
                                    <div 
                                        @click="toRaiseFrenchFries"
                                        class="plus-img"
                                    >
                                        <img src="./../assets/images/second/chevron.svg"/>
                                    </div>
                                    <div class="amount-of-orders-price">
                                        ${{totalFrenchFries}}
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="card-line-tamplate"></div>
                    </template>
                    <template v-if="!isAddSalmonAndVegetables">
                        <div class="card-item-tamplate">
                            <img class="card-img" src="./../assets/images/second/plate__salmon-vegetables.png"/>
                            <div class="numberOfOrders">
                                {{numberSalmonAndVegetables}}
                            </div>
                            <div class="card-info">
                                <div>
                                    Salmon and Vegetables
                                </div>
                                <div class="card-info-price">${{SalmonAndVegetables.price}}</div>
                            
                                <div class="amount-of-orders">
                                    <div 
                                        @click="removeSalmonAndVegetables"
                                        class="minus-img"
                                    > 
                                        <img src="./../assets/images/second/chevron.svg"/>
                                    </div>
                                        {{numberSalmonAndVegetables}}
                                    <div 
                                        @click="toRaiseSalmonAndVegetables"
                                        class="plus-img"
                                    >
                                        <img src="./../assets/images/second/chevron.svg"/>
                                    </div>
                                    <div class="amount-of-orders-price">
                                        ${{totalSalmonAndVegetables}}
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="card-line-tamplate"></div>
                    </template>
                    <template v-if="!isAddSpaghettiWithMeatSauce">
                        <div class="card-item-tamplate">
                            <img class="card-img" src="./../assets/images/second/plate__spaghetti-meat-sauce.png"/>
                            <div class="numberOfOrders">
                                {{numberSalmonAndVegetables}}
                            </div>
                            <div class="card-info">
                                <div>
                                    Salmon and Vegetables
                                </div>
                                <div class="card-info-price">${{SalmonAndVegetables.price}}</div>
                            
                                <div class="amount-of-orders">
                                    <div 
                                        @click="removeSalmonAndVegetables"
                                        class="minus-img"
                                    > 
                                        <img src="./../assets/images/second/chevron.svg"/>
                                    </div>
                                        {{numberSalmonAndVegetables}}
                                    <div 
                                        @click="toRaiseSalmonAndVegetables"
                                        class="plus-img"
                                    >
                                        <img src="./../assets/images/second/chevron.svg"/>
                                    </div>
                                    <div class="amount-of-orders-price">
                                        ${{totalSalmonAndVegetables}}
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="card-line-tamplate"></div>
                    </template>
                    <template v-if="!isAddChickenSaladwithParmesean">
                        <div class="card-item-tamplate">
                            <img class="card-img" src="./../assets/images/second/plate__chicken-salad.png"/>
                            <div class="numberOfOrders">
                                {{numberOfChickenSaladwithParmesean}}
                            </div>
                            <div class="card-info">
                                <div>
                                    Chicken Salad with Parmesean
                                </div>
                                <div class="card-info-price">${{ChickenSaladwithParmesean.price}}</div>
                            
                                <div class="amount-of-orders">
                                    <div 
                                        @click="removeChickenSaladwithParmesean"
                                        class="minus-img"
                                    > 
                                        <img src="./../assets/images/second/chevron.svg"/>
                                    </div>
                                        {{numberOfChickenSaladwithParmesean}}
                                    <div 
                                        @click="toRaiseChickenSaladwithParmesean"
                                        class="plus-img"
                                    >
                                        <img src="./../assets/images/second/chevron.svg"/>
                                    </div>
                                    <div class="amount-of-orders-price">
                                        ${{totalChickenSaladwithParmesean}}
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

        FrenchFries:[
            {price: 2.23},
            {isAdd: true},
            {total: 2.23},
            {number: 1}
        ],
        SalmonAndVegetables: [
            {price: 5.12},
            {isAdd: true},
            {total: 5.12},
            {number: 1}
        ],
        SpaghettiWithMeatSauce: [
            {price: 7.82},
            {isAdd: true},
            {total: 7.82},
            {number: 1}
        ],
        ChickenSaladwithParmesean:[
            {price: 6.98},
            {isAdd: true},
            {total: 6.98},
            {number: 1}
        ],
        FishSticksAndFries:[
            {price: 6.34},
            {isAdd: true},
            {total: 6.34},
            {number: 1}
        ],
        Ravioli:[
            {price: 6.45},
            {isAdd: true},
            {total: 6.45},
            {number: 1}
        ],
        Tortellini:[
            {price: 6.05},
            {isAdd: true},
            {total: 6.05},
            {number: 1}
        ],
        BaconEggsAndToast:[
            {price: 5.99},
            {isAdd: true},
            {total: 5.99},
            {number: 1}
        ],

        isAddFrenchFries: true,
        totalFrenchFries: 2.23,
        numberOfFrenchFries: 1,

        : 5.12,
        isAddSalmonAndVegetables: true,
        totalSalmonAndVegetables: 5.12,
        numberSalmonAndVegetables: 1,

        
        price: 7.82,
        isAddSpaghettiWithMeatSauce: true,
        totalSpaghettiWithMeatSauce: 7.82,
        numberOfSpaghettiWithMeatSauce: 1,

        isAddChickenSaladwithParmesean: true,
        totalChickenSaladwithParmesean: 6.98,
        numberOfChickenSaladwithParmesean: 1,

        price6.34,
        isAddFishSticksAndFries: true,
        totalFishSticksAndFries:6.34,
        numberOfFishSticksAndFries:1,

        price 6.45,
        isAddRavioli:true,
        ptotalRavioli: 6.45,
        numberOfRavioli: 1,

        price 6.05,
        isAddTortellini:true,
        totalTortellini: 6.05,
        numberOfTortellini: 1,

        price: 5.99,
        isAddBaconEggsAndToast: true,
        totalBaconEggsAndToast: 5.99,
        numberOfBaconEggsAndToast: 1,

        orderPrice: 0,
        subtotal: 0,
    }
  },
  methods:{
    addFrenchFries: function(){
        this.isAddFrenchFries = !this.isAddFrenchFries
        if (this.isAddFrenchFries === true){
            var element = document.getElementById("btnFrenchFries")
            element.style.backgroundColor = "#6B00F5";
            this.subtotal = Math.floor((this.subtotal - this.totalFrenchFries)* 100) / 100
        }else if (this.isAddFrenchFries === false){
            var element = document.getElementById("btnFrenchFries")
            element.style.backgroundColor = "black"
            this.subtotal = Math.floor((this.subtotal + this.FrenchFries.price)* 100) / 100
        }
        this.subtotal = Math.floor((this.subtotal + this.orderPrice)* 100) / 100
    },
    addSalmonAndVegetables: function(){
        this.isAddSalmonAndVegetables = !this.isAddSalmonAndVegetables
        if (this.isAddSalmonAndVegetables === true){
            var element = document.getElementById("btnSalmonAndVegetables")
            element.style.backgroundColor = "#6B00F5";
            this.subtotal = Math.floor((this.subtotal - this.totalSalmonAndVegetables)* 100) / 100
        }else if (this.isAddSalmonAndVegetables === false){
            var element = document.getElementById("btnSalmonAndVegetables")
            element.style.backgroundColor = "black"
            this.subtotal = Math.floor((this.subtotal + this.SalmonAndVegetables.price)* 100) / 100
        }
    },
    addSpaghettiWithMeatSauce: function(){
        this.isAddSpaghettiWithMeatSauce = !this.isAddSpaghettiWithMeatSauce
        if (this.isAddSpaghettiWithMeatSauce === true){
            var element = document.getElementById("btnSpaghettiWithMeatSauce")
            element.style.backgroundColor = "#6B00F5";
            this.subtotal = Math.floor((this.subtotal - this.totalSpaghettiWithMeatSauce)* 100) / 100
        }else if (this.isAddSpaghettiWithMeatSauce === false){
            var element = document.getElementById("btnSpaghettiWithMeatSauce")
            element.style.backgroundColor = "black"
            this.subtotal = Math.floor((this.subtotal + this.SpaghettiWithMeatSauce)* 100) / 100
        }
    },
    addChickenSaladwithParmesean: function(){
        this.isAddChickenSaladwithParmesean = !this.isAddChickenSaladwithParmesean
        if (this.isAddChickenSaladwithParmesean === true){
            var element = document.getElementById("btnChickenSaladwithParmesean")
            element.style.backgroundColor = "#6B00F5";
            this.subtotal = Math.floor((this.subtotal - this.totalChickenSaladwithParmesean)* 100) / 100
        }else if (this.isAddChickenSaladwithParmesean === false){
            var element = document.getElementById("btnChickenSaladwithParmesean")
            element.style.backgroundColor = "black"
            this.subtotal = Math.floor((this.subtotal + this.ChickenSaladwithParmesean.price)* 100) / 100
        }
    },
    addFishSticksAndFries: function(){
        this.isAddFishSticksAndFries = !this.isAddFishSticksAndFries
        if (this.isAddFishSticksAndFries === true){
            var element = document.getElementById("btnFishSticksAndFries")
            element.style.backgroundColor = "#6B00F5";
            this.subtotal = Math.floor((this.subtotal - this.totalFishSticksAndFries)* 100) / 100
        }else if (this.isAddFishSticksAndFries === false){
            var element = document.getElementById("btnFishSticksAndFries")
            element.style.backgroundColor = "black"
            this.subtotal = Math.floor((this.subtotal + this.FishSticksAndFries.price)* 100) / 100
        }
    },
    addRavioli: function(){
        this.isAddRavioli = !this.isAddRavioli
        if (this.isAddRavioli === true){
            var element = document.getElementById("btnRavioli")
            element.style.backgroundColor = "#6B00F5";
            this.subtotal = Math.floor((this.subtotal - this.totalRavioli)* 100) / 100
        }else if (this.isAddRavioli === false){
            var element = document.getElementById("btnRavioli")
            element.style.backgroundColor = "black"
            this.subtotal = Math.floor((this.subtotal + this.Ravioli.price)* 100) / 100
        }
    },
    addTortellini: function(){
        this.isAddTortellini = !this.isAddTortellini
        if (this.isAddTortellini === true){
            var element = document.getElementById("btnTortellini")
            element.style.backgroundColor = "#6B00F5";
            this.subtotal = Math.floor((this.subtotal - this.totalTortellini)* 100) / 100
        }else if (this.isAddTortellini === false){
            var element = document.getElementById("btnTortellini")
            element.style.backgroundColor = "black"
            this.subtotal = Math.floor((this.subtotal + this.Tortellini.price)* 100) / 100
        }
    },
    addBaconEggsAndToast: function(){
        this.isAddBaconEggsAndToast = !this.isAddBaconEggsAndToast
        if (this.isAddBaconEggsAndToast === true){
            var element = document.getElementById("btnBaconEggsAndToast")
            element.style.backgroundColor = "#6B00F5";
            this.subtotal = Math.floor((this.subtotal - this.totalBaconEggsAndToast)* 100) / 100
        }else if (this.isAddBaconEggsAndToast === false){
            var element = document.getElementById("btnBaconEggsAndToast")
            element.style.backgroundColor = "black"
            this.subtotal = Math.floor((this.subtotal + this.BaconEggsAndToast)* 100) / 100
        }
    },
    toRaiseFrenchFries: function() {
        this.numberOfFrenchFries = this.numberOfFrenchFries + 1
        this.totalFrenchFries = Math.floor((this.totalFrenchFries + this.FrenchFries.price)* 100) / 100
        this.subtotal = Math.floor((this.subtotal + this.FrenchFries.price)* 100) / 100
    },
    removeFrenchFries: function() {
        if (this.numberOfFrenchFries > 1) {
            this.numberOfFrenchFries = this.numberOfFrenchFries - 1;
            this.totalFrenchFries = Math.floor((this.totalFrenchFries - this.FrenchFries.price)* 100) / 100
            this.subtotal = Math.floor((this.subtotal - this.FrenchFries.price)* 100) / 100
        }else if (this.numberOfFrenchFries === 1){
            this.isAddFrenchFries = true
            var element = document.getElementById("btnFrenchFries");
            element.style.backgroundColor = "#6B00F5";
            this.subtotal = Math.floor((this.subtotal - this.FrenchFries.price)* 100) / 100
        }
    },
    toRaiseSalmonAndVegetables: function() {
        this.numberSalmonAndVegetables = this.numberSalmonAndVegetables + 1
        this.totalSalmonAndVegetables = Math.floor((this.totalSalmonAndVegetables + this.SalmonAndVegetables.price)* 100) / 100
        this.subtotal = Math.floor((this.subtotal + this.SalmonAndVegetables.price)* 100) / 100
    },
    removeSalmonAndVegetables: function() {
        if (this.numberSalmonAndVegetables > 1) {
            this.numberSalmonAndVegetables = this.numberSalmonAndVegetables - 1;
            this.totalSalmonAndVegetables = Math.floor((this.totalSalmonAndVegetables - this.SalmonAndVegetables.price)* 100) / 100
            this.subtotal = this.subtotal - Math.floor((this.SalmonAndVegetables.price)* 100) / 100
        }else if (this.numberSalmonAndVegetables === 1){
            this.isAddSalmonAndVegetables = true
            var element = document.getElementById("btnSalmonAndVegetables")
            element.style.backgroundColor = "#6B00F5";
            this.subtotal = Math.floor((this.subtotal - this.SalmonAndVegetables.price)* 100) / 100
        }
    },
    toRaiseChickenSaladwithParmesean: function() {
        this.numberOfChickenSaladwithParmesean = this.numberOfChickenSaladwithParmesean + 1
        this.totalChickenSaladwithParmesean = Math.floor((this.totalChickenSaladwithParmesean + this.ChickenSaladwithParmesean.price)* 100) / 100
        this.subtotal = Math.floor((this.subtotal + this.ChickenSaladwithParmesean.price)* 100) / 100
    },
    removeChickenSaladwithParmesean: function() {
        if (this.numberOfChickenSaladwithParmesean > 1) {
            this.numberOfChickenSaladwithParmesean = this.numberOfChickenSaladwithParmesean - 1;
            this.totalChickenSaladwithParmesean = Math.floor((this.totalChickenSaladwithParmesean - this.ChickenSaladwithParmesean.price)* 100) / 100
            this.subtotal = Math.floor((this.subtotal - this.ChickenSaladwithParmesean.price)* 100) / 100
        }else if (this.numberOfChickenSaladwithParmesean === 1){
            this.isAddChickenSaladwithParmesean = true
            var element = document.getElementById("btnFrenchFries");
            element.style.backgroundColor = "#6B00F5";
            this.subtotal = Math.floor((this.subtotal - this.ChickenSaladwithParmesean.price)* 100) / 100
        }
    },
  },
}
</script>

<style scoped lang="scss">
@import "./../assets/styles/second.scss";
</style>