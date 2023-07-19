<script setup>
import Home from "@/components/home/Home.vue";
import Markets from "@/components/home/Markets.vue";
import MarketsCard from "@/components/home/MarketsCard.vue";
import Tools from "@/components/home/Tools.vue";
import About from "@/components/home/About.vue";
import FAQ from "@/components/home/FAQ.vue";
import AI from "@/components/home/AI.vue";
import Footer from "@/components/home/Footer.vue";
</script>

<template>
    <Home />
    <Markets />
    <MarketsCard />
    <Tools />
    <About />
    <FAQ />
    <AI />
    <Footer />
</template>

<style lang="scss">
@import 'bootstrap/scss/functions';
@import 'bootstrap/scss/variables';
@import 'bootstrap/scss/mixins';

#app {
    background-image: url("@/assets/img/marble.png");
    background-repeat: repeat;
    background-size: 768px;
}

@include media-breakpoint-up(md) {
    #app {
        background-size: 100%;
    }
}
</style>