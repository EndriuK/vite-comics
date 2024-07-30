<script>

import covers from '../data/covers'
import ProductCard from './ProductCard.vue';

export default {
    components: {
        ProductCard
    },
    data() {
        return {
            covers
        }
    }
}
</script>
<template lang="">
    <main>
        <div class="bg-black">
            <div class="container">
                <div class="row">
                    <div class="col-12">
                        <img class="img-fluid" src="../assets/img/jumbotron.jpg">   
                    </div>
                    <ProductCard v-for="cover, index in covers" :key="`p-${index}`" :cardData="cover"  />
                </div>
            </div>
        </div>
        
        <div class="bg-blue">
            <div class="container">
                <div class="row">
                    <div class="col-12">
                        <ul class="list-unstyled mt-5 justify-content-center d-flex">
                            <li>
                                <a href="/">
                                    <img src="../assets/img/buy-comics-digital-comics.png" >
                                </a>
                                <span>digital comics</span>
                            </li>
                            <li>
                                <a href="/">
                                    <img src="../assets/img/buy-comics-merchandise.png">
                                </a>
                                <span>dc merchandise</span>
                            </li>
                            <li>
                                <a href="/">
                                    <img src="../assets/img/buy-comics-subscriptions.png">
                                </a>
                                <span>subscription</span>
                            </li>
                            <li>
                                <a href="/">
                                    <img src="../assets/img/buy-comics-shop-locator.png">
                                </a>
                                <span>comic shop locator</span>
                            </li>
                            <li>
                                <a href="/">
                                    <img src="../assets/img/buy-dc-power-visa.svg">
                                </a>
                                <span>dc power visa</span>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        
    </main>
</template>
<style lang="scss" scoped>
    .bg-blue {
        background-color:#0282F9;
        color: #fff;
    }
    .bg-black {
        color: #fff;
    }
    ul {
        li{
            padding:20px 15px;
        }

        span {
            margin-left: 10px;
            text-transform: uppercase;
        }
    }

    span {
        font-size: 15px;
    }
</style>