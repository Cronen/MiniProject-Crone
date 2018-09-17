<template>
<div class="mt-5 row">
    <div class="col-md-2"></div>
    <div v-if="product" class="col-md-8 row m-5 proitem">
        <div class="col pull-right">
            <img :src="product.imgUrl" alt="product" class="proitem__img">
        </div>
            <div class="col align-left">
                <h2>{{product.title}}</h2>
                <p>price here</p>
                <p class="f_txt">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam eget arcu sed augue elementum laoreet nec in orci. Fusce luctus finibus tellus eget fringilla. Praesent eget felis consequat, ullamcorper est vel, iaculis odio. Phasellus hendrerit erat ex, at pharetra sem cursus ut. Morbi tempus viverra convallis. Etiam egestas ullamcorper eros, vel aliquam quam sagittis sit amet. Donec suscipit mi vel massa rhoncus, non iaculis velit tempor. Pellentesque ut odio nec leo cursus convallis eu sit amet dolor. Pellentesque eu nibh sollicitudin purus volutpat lacinia a sed elit. In blandit ultricies sapien, nec congue dolor porttitor non. Nullam at bibendum augue, sed mattis sapien.</p>
                <router-link to="/products"> &#8592; Back</router-link>    
            </div>
        </div>
        <div v-else class="col-md-8">
            <h1 class="mt-5">Product not found</h1>
        </div>
    </div>
</template>

<script>
import axios from "axios";

export default {
    data() {
        return {
            product: null
        };
    },
    mounted() {
        this.GetProductById();
    },
    methods: {
        GetProductById() {
            var productId = Number(this.$route.params.id);
            console.log(productId);
            axios.get("/product-data.json")
                .then(response => (this.product = response.data.products.find(p => p.id === productId)))
                .catch(error => console.log(error))
                .finally(console.log("Complete"));
        }
    }
}
</script>
