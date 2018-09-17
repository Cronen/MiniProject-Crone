<template>
<div class="row productBlock justify-content-md-center m-5">
    <div v-for="product in products" :key="product.id" class="col">
        <div class="productBox__Item">
            <router-link :to="{name: 'product', params: {id: product.id}}"><img :src="product.imgUrl" alt="product" class="productBox__sImg"></router-link>
            <h4>{{product.title}}</h4>
        </div>
    </div>
</div>
</template>

<script>
import axios from "axios";

export default {
    data() {
        return {
            products: null
        };
    },
    mounted() {
        this.getData();
    },
    methods: {
        getData() {
            axios
                .get("/product-data.json")
                .then(response => (this.products = response.data.products))
                .catch(error => console.log(error))
                .finally(console.log("Complete"));
        }
    }
};
</script>
