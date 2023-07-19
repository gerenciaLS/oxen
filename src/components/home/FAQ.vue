<script setup>
</script>

<template>
    <div class="position-relative">
        <div class="container-fluid mt-5">
            <div class="row justify-content-center my-5">
                <div class="col-11 col-md-6 text-center title mt-5">
                    FAQ
                </div>
            </div>
            <div class="row mt-md-5 pt-md-5 justify-content-center">
                <div class="col-11 col-md-8">
                    <div class="accordion" id="accordionExample">
                        <div class="accordion-item">
                            <h2 class="accordion-header">
                                <button class="accordion-button" type="button" data-bs-toggle="collapse"
                                    data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
                                    Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu
                                </button>
                            </h2>
                            <div id="collapseOne" class="accordion-collapse collapse show"
                                data-bs-parent="#accordionExample">
                                <div class="accordion-body">
                                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
                                    incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
                                    exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure
                                    dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                                    Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt
                                    mollit anim id est laborum.
                                </div>
                            </div>
                        </div>
                        <div class="accordion-item">
                            <h2 class="accordion-header">
                                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                                    data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
                                    Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu
                                </button>
                            </h2>
                            <div id="collapseTwo" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
                                <div class="accordion-body">
                                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
                                    incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
                                    exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure
                                    dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                                    Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt
                                    mollit anim id est laborum.
                                </div>
                            </div>
                        </div>
                        <div class="accordion-item">
                            <h2 class="accordion-header">
                                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                                    data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
                                    Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu
                                </button>
                            </h2>
                            <div id="collapseThree" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
                                <div class="accordion-body">
                                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
                                    incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
                                    exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure
                                    dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                                    Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt
                                    mollit anim id est laborum.
                                </div>
                            </div>
                        </div>
                        <div class="accordion-item">
                            <h2 class="accordion-header">
                                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                                    data-bs-target="#collapseFourth" aria-expanded="false" aria-controls="collapseFourth">
                                    Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu
                                </button>
                            </h2>
                            <div id="collapseFourth" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
                                <div class="accordion-body">
                                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
                                    incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
                                    exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure
                                    dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                                    Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt
                                    mollit anim id est laborum.
                                </div>
                            </div>
                        </div>
                        <div class="accordion-item">
                            <h2 class="accordion-header">
                                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                                    data-bs-target="#collapseFifth" aria-expanded="false" aria-controls="collapseFifth">
                                    Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu
                                </button>
                            </h2>
                            <div id="collapseFifth" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
                                <div class="accordion-body">
                                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
                                    incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
                                    exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure
                                    dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                                    Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt
                                    mollit anim id est laborum.
                                </div>
                            </div>
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
        color: white;
        position: relative;
        font-weight: 700;
        font-size: 25px;
        width: 700px;

        &::after {
            border: $primary solid 1px;
            position: absolute;
            bottom: -15px;
            left: calc(50% - 100px / 2);
            width: 100px;
            content: "";
        }
    }

    .accordion {
        .accordion-item {
            background-color: transparent;
            border: none;
            border-radius: 0;
            border-bottom: 1px solid $primary;

            .accordion-button {
                background-color: transparent;
                color: $primary;
                box-shadow: none;
                border-bottom: 1px solid $primary;
                font-size: 13px;
                padding: 20px 0;
                padding-left: 0;
                padding-right: 1rem;
                font-weight: 600;

                &.collapsed {
                    color: white;
                    font-weight: 500;
                    border-bottom: none;
                }

                &::after {
                    background-image: url("@/assets/img/arrow.svg");
                }
            }

            .accordion-collapse {
                color: white;

                .accordion-body {
                    font-size: 12px;
                    font-weight: 300;
                    text-align: justify;
                }
            }
        }
    }

}

@include media-breakpoint-up(md) {
    .accordion {
        .accordion-item {
            .accordion-a {
                font-size: 20px;
            }

            .accordion-collapse {
                .accordion-body {
                    padding-left: 2rem;
                    padding-right: 6rem;
                    font-size: 16px
                }
            }
        }
    }
}

@include media-breakpoint-up(xxl) {}
</style>
