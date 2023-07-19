<script setup>
</script>

<template>
    <div class="position-relative">
        <div class="bg-img-mask position-absolute w-100"></div>
        <div class="container-fluid mt-5 border-top border-primary">
            <div class="row justify-content-center py-1 py-md-0 mb-md-5 pt-md-5">
                <div class="col-4 d-none d-md-block">
                    <div class="col-10 col-xxl-9">
                        <img class="mb-4" src="@/assets/logo.png" />
                        <div class="footer-link">
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
                            labore
                            et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi
                            ut
                            aliquip ex ea commodo consequat.
                        </div>
                    </div>
                </div>
                <div class="col-2 d-none d-md-block">
                    <div class="footer-title">Links Úteis</div>
                    <ul class="list-unstyled h-100 d-flex flex-column">
                        <li class="mb-3">
                            <a class="text-decoration-none footer-link" href="#">
                                Serviços
                            </a>
                        </li>
                        <li class="mb-3">
                            <a class="text-decoration-none footer-link" href="#">
                                Quem somos
                            </a>
                        </li>
                        <li class="mb-auto">
                            <a class="text-decoration-none footer-link" href="#">
                                Suporte
                            </a>
                        </li>
                    </ul>
                </div>
                <div class="col-2 d-none d-md-block">
                    <div class="footer-title">LGPD</div>
                    <ul class="list-unstyled h-100 d-flex flex-column">
                        <li class="mb-3">
                            <a class="text-decoration-none footer-link" href="#">
                                Termos de Uso
                            </a>
                        </li>
                        <li class="mb-auto">
                            <a class="text-decoration-none footer-link" href="#">
                                Política Privacidade
                            </a>
                        </li>
                    </ul>

                </div>
                <div class="col-12 col-md-1">
                    <div class="footer-title d-none d-md-block">Informações</div>
                    <ul class="list-unstyled h-100 d-flex flex-md-column">
                        <li class="mb-md-2 me-3 me-md-0 my-auto my-md-0">
                            <a class="text-decoration-none d-flex" href="tel:(41) 9977-53206">
                                <i class="bi bi-whatsapp text-primary me-2"></i>
                                <span class="text-nowrap footer-link">(41) 9977-53206</span>
                            </a>
                        </li>
                        <li class="mb-md-3 my-auto my-md-0">
                            <a class="text-decoration-none d-flex" href="mailto:email@email.com">
                                <i class="bi bi-envelope text-primary me-2"></i>
                                <span class="footer-link">email@email.com</span>
                            </a>
                        </li>
                        <li class="mb-auto ms-auto ms-md-0 my-auto my-md-0">
                            <div class="d-flex">
                                <a class="rounded-circle bg-primary position-relative me-2 p-3" href="#">
                                    <i class="bi bi-instagram position-absolute"></i>
                                </a>
                                <a class="rounded-circle bg-primary position-relative p-3" href="#">

                                    <i class="bi bi-facebook position-absolute"></i>
                                </a>
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
        <div class="footer-banner text-center bg-primary py-4 d-none d-md-block">
            desenvolvido por ycnataz
        </div>
    </div>
</template>

<style lang="scss" scoped>
@import "@/assets/scss/custom.scss";
@import 'bootstrap/scss/functions';
@import 'bootstrap/scss/variables';
@import 'bootstrap/scss/mixins';

.bg-img-mask {
    background-color: black;
    background-size: 100%;
    height: 100%;
    opacity: .5;
}

.container-fluid {
    position: relative;

    .footer-title {
        color: white;
        margin-bottom: 20px;
        font-size: 14px;
        font-weight: 700;
    }

    .footer-link {
        color: white;
        font-size: 13px;
        font-weight: 300;
        color: white;
    }
}

.bi {
    color: white;
    top: 15.5%;
    left: 25%;
}

@include media-breakpoint-up(md) {
    .container-fluid {
        .footer-title {
            font-size: 18px;
            font-weight: 700;
        }

        .footer-link {
            font-size: 14px;
            font-weight: 300;
        }
    }

    .bi {
        top: 15.5%;
        left: 25%;
    }

    .footer-banner {
        position: relative;
        font-size: 10px;
        font-weight: 600;
        letter-spacing: 1.3em;
        color: white;
    }
}

@include media-breakpoint-up(xxl) {}
</style>
