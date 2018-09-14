<template>
<div id="app">
    <top-bar></top-bar>
    <div class="container-fluid">
        <router-view />
    </div>
    <footerbar></footerbar>
</div>
</template>

<script>
import topBar from "./components/top-bar.vue";
import footerbar from "./components/footerbar.vue";

export default {
  name: "app",
  components: {
    topBar,
    footerbar
  }
};
</script>

<style lang="sass">
@import "./assets/scss/styles.scss"
</style>
