<script setup>
import { onMounted } from 'vue';


onMounted(() => {
    let element = document.querySelectorAll(".nav-link");
    element.forEach(e => e.addEventListener("click", (e) => {
        element.forEach(e => e.classList.remove("active"));
        e.target.classList.add("active");
    }));
});

</script>

<template>
    <nav class="navbar navbar-expand-lg position-absolute fixed-top">
        <div class="container-fluid mt-md-4 pt-md-4 mt-xxl-5 pt-xxl-5">
            <a class="navbar-brand" href="#">
                <img src="@/assets/logo.png" :height="20" />
            </a>
            <div class="d-flex align-items-center">
                <a class="text-decoration-none d-md-none me-3" href="#">
                    <i class="bi bi-person-fill me-1"></i> Login
                </a>
                <a class="navbar-toggler shadow-none border-0" type="button" data-bs-toggle="offcanvas"
                    data-bs-target="#offcanvas" aria-controls="" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="bi bi-list display-3 text-primary"></span>
                </a>
            </div>
            <div class="offcanvas offcanvas-top bg-black h-100" tabindex="-1" id="offcanvas"
                aria-labelledby="offcanvasLabel">
                <div class="offcanvas-body">
                    <ul class="navbar-nav ms-auto mt-3 mt-md-0">
                        <li class="nav-item text-uppercase">
                            <a class="nav-link active" aria-current="page" href="#">Home</a>
                        </li>
                        <li class="nav-item text-uppercase">
                            <a class="nav-link" href="#">Markets</a>
                        </li>
                        <li class="nav-item text-uppercase">
                            <a class="nav-link" href="#">Tools</a>
                        </li>
                        <li class="nav-item text-uppercase">
                            <a class="nav-link" href="#">AI</a>
                        </li>
                        <li class="nav-item text-uppercase d-none d-md-block">
                            <a class="btn btn-primary text-white rounded-pill py-0" href="#">
                                <i class="bi bi-person-fill me-1"></i> Login
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </nav>
</template>

<style lang="scss" scoped>
@import "@/assets/scss/custom.scss";
@import "bootstrap/scss/_functions.scss";
@import "bootstrap/scss/_variables.scss";
@import 'bootstrap/scss/mixins';

.container-fluid {
    .navbar-brand>img {
        height: 20px;
    }
    
    .offcanvas {
        .offcanvas-body {
            margin-top: 56px;
        }

        .nav-link {
            color: white;
            text-align: end;
            margin-right: 12px;
        }
    }
}

@include media-breakpoint-up(md) {

    .container-fluid {
        margin: 0 10%;

        .navbar-brand>img {
            height: 45px;
        }

        .offcanvas {
            .offcanvas-body {
                margin-top: 0px;
            }

            .navbar-nav {
                .nav-item {
                    margin: 0 20px;
                    align-self: center;

                    &:last-child {
                        margin-left: 40px;
                        margin-right: 0;
                    }

                    .nav-link {
                        font-family: Montserrat;
                        font-size: 12px;
                        font-weight: 100;
                        letter-spacing: 1px;
                        text-align: left;
                        color: white;

                        &.active {
                            color: $primary;
                            font-weight: 400;
                        }
                    }

                    .btn {
                        font-size: 12px;
                        line-height: 2rem;
                    }
                }
            }
        }
    }


}

@include media-breakpoint-up(xxl) {


    .nav-link,
    .btn {
        font-size: 14px;
    }

    .navbar-brand>img {
        height: 40px;
    }
}
</style>