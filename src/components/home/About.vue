<script setup>
</script>

<template>
    <div class="position-relative">
        <div class="bg-img position-absolute w-100"></div>
        <div class="bg-img-mask position-absolute w-100"></div>
        <div class="container-fluid mt-5 py-5">
            <div class="row justify-content-center mt-md-5 mb-5">
                    <div class="col-11 text-center title mt-xxl-5">Solidity and experience</div>
            </div>
            <div class="row justify-content-center col-md-8 mx-md-auto">
                <div class="col-12 col-md-4 text-center mb-3 mb-md-0">
                    <div class="item-title">Custody</div>
                    <div class="item-subtitle">+ 99 million</div>
                </div>
                <div class="col-12 col-md-4 text-center mb-3 mb-md-0">
                    <div class="item-title">Customers</div>
                    <div class="item-subtitle">+ 6K</div>
                </div>
                <div class="col-12 col-md-4 text-center">
                    <div class="item-title">Transactions</div>
                    <div class="item-subtitle">+ 2 million</div>
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

.bg-img {
    background-image: url("@/assets/img/flow-mobile.png");
    background-repeat: no-repeat;
    background-size: 100%;
    height: 300%;
    top: -325px;
}

.bg-img-mask {
    content: url("@/assets/img/flow-gradient.png");
    background-repeat: no-repeat;
    background-size: 100%;
    height: 316px;
}

.container-fluid {
    position: relative;
    .title {
        position: relative;
        font-size: 25px;
        font-weight: 700;
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

    .item-title {
        font-size: 16px;
        font-weight: 700;
        color: white;
    }

    .item-subtitle {
        font-size: 32px;
        font-weight: 300;
        color: white;
    }
}

@include media-breakpoint-up(md) {
    .bg-img {
        background-image: url("@/assets/img/flow.png");
        height: 665px;
        top: -175px
    }

    .bg-img-mask {
        top: 30px
    }

    .container-fluid {
        .title {
            font-size: 32px;
        }

        .item-title {
            font-size: 32px;
        }

        .item-subtitle {
            font-size: 48px;
        }
    }
}

@include media-breakpoint-up(xxl) {
    .bg-img-mask {
        top: 80px
    }

    .container-fluid {
        .title {
            font-size: 48px;
        }

        .item-title {
            font-size: 32px;
        }

        .item-subtitle {
            font-size: 64px;
        }
    }
}
</style>
