<script setup>
</script>

<template>
    <div class="position-relative">
        <div class="container-fluid pb-md-5">
            <div class="row justify-content-center my-5">
                <div class="col-11 col-md-6 text-center title mt-5">
                    Trade with AI support
                </div>
            </div>
            <div class="row mt-md-5 pt-md-5 justify-content-center">
                <div class="col-11 col-md-3 mb-5 mb-md-0">
                    <div class="row">
                        <div class="col-2 col-md-12 d-flex">
                            <img class="item-img m-auto me-3 me-md-auto mb-md-4" src="../../assets/img/horse.svg" />
                        </div>
                        <div class="col-10 col-md-12">
                            <div class="item-title mb-2">Pratice your strategy</div>
                            <div class="item-paragraph">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                                eiusmod
                                tempor incididunt ut labore
                                et dolore magna aliqua. Ut enim ad minim veniam</div>
                        </div>
                    </div>
                </div>
                <div class="col-11 col-md-3 mb-5 mb-md-0">
                    <div class="row">
                        <div class="col-2 col-md-12 d-flex">
                            <img class="item-img m-auto me-3 me-md-auto mb-md-4" src="../../assets/img/atom.svg" />
                        </div>
                        <div class="col-10 col-md-12">
                            <div class="item-title mb-2">Pratice your strategy</div>
                            <div class="item-paragraph">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                                eiusmod
                                tempor incididunt ut labore
                                et dolore magna aliqua. Ut enim ad minim veniam</div>
                        </div>
                    </div>
                </div>
                <div class="col-11 col-md-3">
                    <div class="row">
                        <div class="col-2 col-md-12 d-flex">
                            <img class="item-img m-auto me-3 me-md-auto mb-md-4" src="../../assets/img/graphics.svg" />
                        </div>
                        <div class="col-10 col-md-12">
                            <div class="item-title mb-2">Pratice your strategy</div>
                            <div class="item-paragraph">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                                eiusmod
                                tempor incididunt ut labore
                                et dolore magna aliqua. Ut enim ad minim veniam</div>
                        </div>
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
    .title {
        position: relative;
        font-weight: 700;
        font-size: 25px;
        width: 700px;
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

    .item-img {
        height: 40px;
    }

    .item-title {
        color: white;
        font-size: 18px;
        font-weight: 700;
        text-align: left;

    }

    .item-paragraph {
        color: white;
        font-size: 12px;
        font-weight: 400;
        text-align: left;

    }
}

@include media-breakpoint-up(md) {
    .container-fluid {
        .title {
            font-weight: 700;
            font-size: 25px;
            width: 700px;

            &::after {
                bottom: -15px;
                // left: 42.86%;
                width: 100px;
            }
        }

        .item-img {
            height: 100px;
        }

        .item-title {
            font-size: 18px;
            font-weight: 700;
            text-align: center;

        }

        .item-paragraph {
            font-size: 12px;
            font-weight: 400;
            text-align: center;

        }
    }

}

@include media-breakpoint-up(xxl) {}
</style>
