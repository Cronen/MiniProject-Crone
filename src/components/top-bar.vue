<template>
<header class="container-fluid headblock">
    <div class="headblock row text-nowrap">
        <div class="col-md-2"></div>
        <div class="col-md-1 headblock__item">Currency: GP</div>
        <div class="col-md-3"></div>
        <div class="headblock__item col-md-2 row">
            <div class="col-md-3">
                <router-link to="/register">Register</router-link>
            </div>
            <div class="col-md-3">
                <router-link to="/">Sign in</router-link>
            </div>
        </div>
        <div class="col-md-1 headblock__item--card">
            <div class="float-center"><i class="fa fa-shopping-cart ml-4"></i> empty</div>
        </div>
        <div class="col-md-2"></div>

    </div>
    <div class="row m-4 navigate">
        <div class="col-md-1"></div>
        <div class="col-md-2">
            <router-link to="/"><img src="@/assets/img/logo.png" alt="logo"></router-link>
        </div>
        <div class="col-md-2"></div>
        <div class="col-md-5 navigate__item float-right row">
            <p class="col navigation__item--link">
                <router-link to="/products">mens</router-link>
            </p>
            <p class="col navigation__item--link">
                <router-link to="/products">womens</router-link>
            </p>
            <p class="col navigation__item--link">
                <router-link to="/brand">the brand</router-link>
            </p>
            <p class="col">local stores</p>
            <p class="col">look book</p>
        </div>
        <div class="col-md-2">
            <input type="text" placeholder="Search.."><i class="fa fa-search ml-2"></i>
        </div>
    </div>
</header>
</template>

<script>
export default {
    name: "topBar"
};
</script>
