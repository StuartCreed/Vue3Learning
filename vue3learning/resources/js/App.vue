<template>
    <section class="app flex flex-col">
        <Header></Header>
        <Main></Main>
        <Footer></Footer>
    </section>
</template>

<script>
import Footer from "./components/Footer";
import Header from "./components/Header/Header";
import Main from "./components/Main";

export default {
    name: "App.vue",
    components: {Header, Footer, Main}
}
</script>

<style scoped>
    .app {
        --theme-color-one: pink;
        --theme-color-two: orange;
        --active: olive
    }
</style>
