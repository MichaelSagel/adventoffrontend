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
                    <img class="menu-img" src="./../assets/images/second/plate__french-fries.png" />
                    <div class="menu-item-info">
                        <div
                            class="menu-title"
                        >
                            French Fries with Ketchup
                        </div>
                        <div 
                            class="price"
                        >
                            $2.23
                        </div>
                        <div
                            class="btn-bay"
                            id="myDiv"
                            @click="bought"
                        >
                            <template v-if="isBought">
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
                <div class="menu-item pale-rose">
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
                            $5.12
                        </div>
                        <div
                            class="btn-bay"
                            id="myDiv"
                            @click="bought"
                        >
                            <template v-if="isBought">
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
                            $7.82
                        </div>
                        <div
                            class="btn-bay"
                            id="myDiv"
                            @click="bought"
                        >
                            <template v-if="isBought">
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
                            $6.98
                        </div>
                        <div
                            class="btn-bay"
                            id="myDiv"
                            @click="bought"
                        >
                            <template v-if="isBought">
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
                            $6.34
                        </div>
                        <div
                            class="btn-bay"
                            id="myDiv"
                            @click="bought"
                        >
                            <template v-if="isBought">
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
                            $6.45
                        </div>
                        <div
                            class="btn-bay"
                            id="myDiv"
                            @click="bought"
                        >
                            <template v-if="isBought">
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
                            $6.05
                        </div>
                        <div
                            class="btn-bay"
                            id="myDiv"
                            @click="bought"
                        >
                            <template v-if="isBought">
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
                            $5.99
                        </div>
                        <div
                            class="btn-bay"
                            id="myDiv"
                            @click="bought"
                        >
                            <template v-if="isBought">
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

        <div class="card"
        >
        </div>
    </div>
</template>


<script>
    
export default {
    colorMode: "second",
    data: function () {
    return {
      isBought: true,
    }
  },
  methods:{
    bought: function(){
        this.isBought = !this.isBought
        if (this.isBought === true){
            var element = document.getElementById("myDiv");
            element.style.backgroundColor = "#6B00F5";
        }else if (this.isBought === false){
            var element = document.getElementById("myDiv");
            element.style.backgroundColor = "black";
        }
    }
  },
}
</script>


<style scoped lang="scss">
@import "./../assets/styles/second.scss";
</style>





