<script setup>
</script>

<template>
    <div class="position-relative">
        <div class="container-fluid py-5">
            <div class="row justify-content-center align-items-center">
                <div class="col-11 col-md-6">
                    <div class="title">
                        A world of opportunities with Global Markets
                    </div>
                    <div class="mb-5 paragraph">
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
                        et dolore magna aliqua. Ut enim ad minim veniam
                    </div>
                    <div class="mb-5 paragraph">
                        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
                        et dolore magna aliqua. Ut enim ad minim veniam
                    </div>
                    <div class="d-flex w-100 justify-content-center justify-content-md-start ">
                        <a class="col-8 col-md-3 py-2 btn btn-primary rounded-pill text-white">
                            <span class="me-2">Label</span>
                            <i class="bi bi-arrow-right"></i>
                        </a>
                    </div>
                </div>
                <div class="col-11 col-md-6">
                    <div class="d-flex w-100 justify-content-center align-items-center py-md-5">
                        <img class="img-creditcard" />
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

.img-creditcard {
    content: url("@/assets/img/creditcard.png");
    height: 341px;
}

.container-fluid {
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
}

@include media-breakpoint-up(md) {
    .img-creditcard {
        height: 540px;
    }

    .container-fluid {
        width: 80%;

        .title {
            position: relative;
            font-weight: 700;
            font-size: 34px;
            text-align: left;
            margin-bottom: 72px;

            &::after {
                border: $primary solid 1px;
                position: absolute;
                bottom: -29px;
                left: 0;
                width: 150px;
                content: "";
            }
        }

        .paragraph {
            font-size: 11px;
            line-height: 20px;
            text-align: left;
            width: 470px;
        }
    }
}

@include media-breakpoint-up(xxl) {
    .img-creditcard {
        height: 750px;
    }

    .container-fluid {
        .title {
            font-size: 48px;
            margin-bottom: 100px;

            &::after {
                border: $primary solid 1px;
                bottom: -40px;
                width: 150px;
                left: 0;
            }
        }

        .paragraph {
            font-size: 15px;
            line-height: 20px;
            width: 650px;
        }
    }
}
</style>
