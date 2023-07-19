<script setup>
</script>

<template>
    <div class="position-relative">
        <div class="bg-img-mask position-absolute w-100"></div>
        <div class="container-fluid pt-3 pt-md-5 pb-5 pb-md-0">
            <div class="row justify-content-center my-5">
                <div class="col-11 col-md-6 text-center title">
                    A world of opportunities with Global Markets
                </div>
            </div>
            <div class="row mt-md-5 pt-md-5 justify-content-center">
                <div class="col-11 col-md-6 mb-3 px-md-3 mb-md-5">
                    <div class="card">
                        <div class="card-body">
                            <div class="row h-100">
                                <div class="col-2 text-nowrap">
                                    <div class="d-flex align-items-center">
                                        <i class="bi bi-cash text-primary"></i>
                                    </div>
                                </div>
                                <div class="col-9 align-self-center">
                                    <div class="text-primary card-title">LOREM ISPUM</div>
                                    <div class="card-paragraph">Ut enim ad minim veniam, quis nostrud
                                        exercitation
                                        ullamco laboris nisi ut aliquip ex ea commodo consequat.</div>
                                </div>
                                <div class="col-1 align-self-end">
                                    <i class="bi bi-arrow-right-short text-primary fs-1"></i>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-11 col-md-6 mt-2 mb-3 px-md-3 mt-md-0 mb-md-5">
                    <div class="card">
                        <div class="card-body">
                            <div class="row h-100">
                                <div class="col-2 text-nowrap">
                                    <div class="d-flex align-items-center">
                                        <i class="bi bi-coin text-primary"></i>
                                    </div>
                                </div>
                                <div class="col-9 align-self-center">
                                    <div class="text-primary card-title">LOREM ISPUM</div>
                                    <div class="card-paragraph">Ut enim ad minim veniam, quis nostrud
                                        exercitation
                                        ullamco laboris nisi ut aliquip ex ea commodo consequat.</div>
                                </div>
                                <div class="col-1 align-self-end">
                                    <i class="bi bi-arrow-right-short text-primary fs-1"></i>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-11 col-md-6 mt-2 mb-3 px-md-3 mt-md-2 mb-md-0">
                    <div class="card">
                        <div class="card-body">
                            <div class="row h-100">
                                <div class="col-2 text-nowrap">
                                    <div class="d-flex align-items-center">
                                        <i class="bi bi-cash text-primary"></i>
                                    </div>
                                </div>
                                <div class="col-9 align-self-center">
                                    <div class="text-primary card-title">LOREM ISPUM</div>
                                    <div class="card-paragraph">Ut enim ad minim veniam, quis nostrud
                                        exercitation
                                        ullamco laboris nisi ut aliquip ex ea commodo consequat.</div>
                                </div>
                                <div class="col-1 align-self-end">
                                    <i class="bi bi-arrow-right-short text-primary fs-1"></i>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-11 col-md-6 mt-2 px-md-3 mt-md-2">
                    <div class="card">
                        <div class="card-body">
                            <div class="row h-100">
                                <div class="col-2 text-nowrap">
                                    <div class="d-flex align-items-center">
                                        <i class="bi bi-coin text-primary"></i>
                                    </div>
                                </div>
                                <div class="col-9 align-self-center">
                                    <div class="text-primary card-title">LOREM ISPUM</div>
                                    <div class="card-paragraph">Ut enim ad minim veniam, quis nostrud
                                        exercitation
                                        ullamco laboris nisi ut aliquip ex ea commodo consequat.</div>
                                </div>
                                <div class="col-1 align-self-end">
                                    <i class="bi bi-arrow-right-short text-primary fs-1"></i>
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

.bg-img-mask {
    background-image: url("@/assets/img/marble-gradient.png");
    background-repeat: no-repeat;
    background-size: 475%;
    height: 400%;
    z-index: -9;
}

.container-fluid {
    .title {
        position: relative;
        font-weight: 700;
        font-size: 25px;
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

    .card {
        height: 102px;
        border-radius: 24px;
        background: linear-gradient(0deg, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0.05)),
            linear-gradient(0deg, rgba(255, 255, 255, 0.01), rgba(255, 255, 255, 0.01));

        border: 1px solid #FFFFFF03;

        &::before {
            width: 28px;
            border: $primary solid 3px;
            position: absolute;
            top: -3px;
            content: "";
        }

        &::after {
            width: 28px;
            border: $primary solid 3px;
            position: absolute;
            bottom: -3px;
            right: 0;
            content: "";
        }

        .bi-cash,
        .bi-coin {
            font-size: 30px;
            position: absolute;
            top: 15%;
        }

        .bi-arrow-right-short {
            font-size: 18px;
            position: absolute;
            bottom: 0%;
            right: 5%;
        }

        .card-title {
            font-weight: 700;
            font-size: 13px;
        }

        .card-paragraph {
            font-weight: 400;
            font-size: 10px;
            color: white;
        }
    }
}

@include media-breakpoint-up(md) {

    .bg-img-mask {
        background-size: 100%;
    }

    .container-fluid {
        width: 80%;

        .title {
            position: relative;
            font-weight: 700;
            font-size: 34px;

            &::after {
                border: $primary solid 1px;
                position: absolute;
                bottom: -29px;
                left: calc(50% - 150px / 2);
                width: 150px;
                content: "";
            }
        }

        .card {
            height: 118px;
            border-radius: 36px;

            &::before {
                width: 38px;
                border: $primary solid 4px;
                position: absolute;
                top: -4px;
                content: "";
            }

            &::after {
                width: 38px;
                border: $primary solid 4px;
                position: absolute;
                bottom: -4px;
                right: 0;
                content: "";
            }

            .bi-cash,
            .bi-coin {
                font-size: 36px;
                position: absolute;
                top: 10%;
                left: 5%;
            }

            .bi-arrow-right-short {
                position: absolute;
                bottom: 5%;
                right: 5%;
            }

            .card-title {
                font-weight: 700;
                font-size: 14px;
            }

            .card-paragraph {
                font-weight: 400;
                font-size: 12px;
            }
        }
    }
}

@include media-breakpoint-up(xxl) {
    .container-fluid {
        .title {
            font-size: 48px;
        }

        .card {
            height: 165px;

            &::before {
                width: 53px;
                border: $primary solid 5.5px;
                top: -6px;
            }

            &::after {
                width: 53px;
                border: $primary solid 5.5px;
                bottom: -6px;
            }

            .bi-cash,
            .bi-coin {
                font-size: 50px;
                top: 10%;
                left: 5%;
            }

            .bi-arrow-right-short {
                bottom: 5%;
                right: 5%;
            }

            .card-title {
                font-size: 20px;
            }

            .card-paragraph {
                font-size: 16px;
            }
        }
    }
}
</style>
