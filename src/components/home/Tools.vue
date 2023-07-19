<script setup>
</script>

<template>
    <div class="position-relative">
        <div class="container-fluid py-5">
            <div class="row justify-content-center align-items-center">
                <div class="col-11">
                    <div class="title mx-auto">
                        A world of opportunities with Global Markets
                    </div>
                    <div class="mb-5 paragraph">
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
                        et dolore magna aliqua. Ut enim ad minim veniam
                    </div>
                    <div class="d-md-none paragraph mb-5">
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
                        et dolore magna aliqua. Ut enim ad minim veniam
                    </div>
                </div>
            </div>
            <!-- DESKTOP -->
            <div class="row justify-content-center align-items-center d-md-none">
                <div class="col-11">
                    <a class="w-100 btn rounded-pill border-primary text-white px-1 mb-3" href="#">Lorem ipsum dolor sit amet
                        consectetur</a>
                    <a class="w-100 btn rounded-pill border-primary text-white px-1 mb-3" href="#">Lorem ipsum dolor sit amet
                        consectetur</a>
                    <a class="w-100 btn rounded-pill border-primary text-white px-1 mb-3" href="#">Lorem ipsum dolor sit amet
                        consectetur</a>
                    <a class="w-100 btn rounded-pill border-primary text-white px-1 mb-3" href="#">Lorem ipsum dolor sit amet
                        consectetur</a>
                    <a class="w-100 btn rounded-pill border-primary text-white px-1" href="#">Lorem ipsum dolor sit amet
                        consectetur</a>
                </div>
            </div>
            <!-- MOBILE -->
            <div class="row justify-content-center align-items-center d-none d-md-flex my-5 pb-5">
                <div class="col-3">
                    <div class="d-flex">
                        <a class="col-2 btn btn-primary rounded-pill shadow-none mx-auto mb-4" href="#"></a>
                    </div>
                    <div class="text-center description">Lorem ipsum dolor sit amet, consectetur adipiscing elit
                    </div>
                </div>
                <div class="col-3">
                    <div class="d-flex">
                        <a class="col-2 btn btn-primary rounded-pill shadow-none mx-auto mb-4" href="#"></a>
                    </div>
                    <div class="text-center description">Lorem ipsum dolor sit amet, consectetur adipiscing elit
                    </div>
                </div>
                <div class="col-3">
                    <div class="d-flex">
                        <a class="col-2 btn btn-primary rounded-pill shadow-none mx-auto mb-4" href="#"></a>
                    </div>
                    <div class="text-center description">Lorem ipsum dolor sit amet, consectetur adipiscing elit
                    </div>
                </div>
                <div class="col-3">
                    <div class="d-flex">
                        <a class="col-2 btn btn-primary rounded-pill shadow-none mx-auto mb-4" href="#"></a>
                    </div>
                    <div class="text-center description">Lorem ipsum dolor sit amet, consectetur adipiscing elit
                    </div>
                </div>
            </div>
            <div class="row justify-content-center align-items-center d-none d-md-flex mb-5">
                <div class="col-3">
                    <div class="d-flex">
                        <a class="col-2 btn btn-primary rounded-pill shadow-none mx-auto mb-4" href="#"></a>
                    </div>
                    <div class="text-center description">Lorem ipsum dolor sit amet, consectetur adipiscing elit
                    </div>
                </div>
                <div class="col-3">
                    <div class="d-flex">
                        <a class="col-2 btn btn-primary rounded-pill shadow-none mx-auto mb-4" href="#"></a>
                    </div>
                    <div class="text-center description">Lorem ipsum dolor sit amet, consectetur adipiscing elit
                    </div>
                </div>
                <div class="col-3">
                    <div class="d-flex">
                        <a class="col-2 btn btn-primary rounded-pill shadow-none mx-auto mb-4" href="#"></a>
                    </div>
                    <div class="text-center description">Lorem ipsum dolor sit amet, consectetur adipiscing elit
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@import "@/assets/scss/custom.scss";
@import 'bootstrap/scss/functions';
@import 'bootstrap/scss/variables';
@import 'bootstrap/scss/mixins';

.container-fluid {
    z-index: 1;
    position: relative;
    .title {
        position: relative;
        font-weight: 700;
        font-size: 25px;
        text-align: center;
        margin-bottom: 50px;
        color: white;


        &::after {
            border: $primary solid 1px;
            position: absolute;
            bottom: -15px;
            left: calc(50% - 100px / 2);
            width: 100px;
            content: "";
        }
    }

    .paragraph {
        color: white;
        font-size: 10px;
        line-height: 20px;
        text-align: center;
    }

    .btn {
        font-size: 10px;
    }
}

@include media-breakpoint-up(md) {
    .container-fluid {
        width: 80%;

        .title {
            position: relative;
            font-weight: 700;
            font-size: 48px;
            margin-bottom: 100px;
            width: 700px;

            &::after {
                border: $primary solid 1px;
                position: absolute;
                bottom: -30px;
                left: calc(50% - 150px / 2);
                width: 150px;
                content: "";
            }
        }

        .paragraph {
            font-size: 15px;
            line-height: 20px;
        }

        .description {
            color: white;
            font-size: 16px;
        }
    }
}
</style>
