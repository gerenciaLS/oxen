<script setup>
import Navbar from '@/components/Navbar.vue'
</script>

<template>
    <div class="bg-img vh-100 position-relative overflow-hidden">
        <navbar />
        <img class="bull-img position-absolute" />
        <div class="mx-4 text-block position-absolute">
            <div class="position-relative mb-4">
                <div class="title">lorem ipsum</div>
                <div class="position-absolute fw-semibold text-primary subtitle">
                    SED DO ESIUMOD TEMPOR
                </div>
            </div>
            <div class="mb-4 paragraph">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
                dolore magna aliqua. Ut enim ad minim veniam.
            </div>
            <a class="col-5 btn btn-black rounded-pill border-white text-white" href="#">
                <span class="me-2">Label</span>
                <i class="bi bi-arrow-right"></i>
            </a>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@import 'bootstrap/scss/functions';
@import 'bootstrap/scss/variables';
@import 'bootstrap/scss/mixins';

.bg-img {
    background-image: url("@/assets/img/chart-mobile.png");
    background-repeat: no-repeat;
    background-size: 100%;
    height: 100%;
    background-color: black;
}

.bull-img {
    content: url("@/assets/img/bull.png");
    background-size: 100px;
    height: 376px;
    left: -10%;
    top: 23%;
}

.text-block {
    top: 63%;

    .title {
        font-family: "bebas neue";
        font-size: 4rem;
        line-height: 4rem;
        background: linear-gradient(180deg, #C39B5E 0%, rgba(195, 155, 94, 0) 85%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
    }

    .subtitle {
        bottom: 0;
        font-size: 18px;
    }

    .paragraph {
        color: white;
        font-size: 10px;
        line-height: 26px;
    }
}

@include media-breakpoint-up(md) {
    .bg-img {
        background-image: url("@/assets/img/chart.png");
        background-repeat: no-repeat;
        background-size: 100%;
    }

    .bull-img {
        height: 70%;
        left: unset;
        right: 10%;
        top: 31%;
    }

    .text-block {
        top: 53%;
        left: 9.2%;
        width: 400px;

        .title {
            font-size: 5.7rem;
            line-height: 5.7rem;
        }

        .subtitle {
            bottom: -8px;
            font-size: 26px;
        }

        .paragraph {
            font-size: 11.5px;
            line-height: 23px;
        }
    }
}

@include media-breakpoint-up(xxl) {
    .text-block {
        width: 550px;

        .title {
            font-size: 8rem;
            line-height: 8rem;
        }

        .subtitle {
            bottom: -9px;
            font-size: 37px;
        }

        .paragraph {
            font-size: 16px;
            line-height: 33px;
        }
    }
}
</style>
