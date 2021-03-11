<template>
    <section class="app">
        <Header></Header>
        <Footer></Footer>
    </section>
</template>

<script>
import Footer from "./components/Footer";
import Header from "./components/Header";
export default {
    name: "app.vue",
    components: {Header, Footer}
}
</script>

<style scoped>
    .app {
        --theme-color-one: pink;
        --theme-color-two: orange;
    }
</style>
