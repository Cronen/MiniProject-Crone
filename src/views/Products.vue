<template>
<div class="mt-5">
    <h2>List of products</h2>
    <product-list />
</div>
</template>

<script>
import ProductList from "@/components/productlist.vue";
export default {
    name: "Home",
    components:{
        ProductList
    }
};
</script>
