<template>
    <div class="main-hero">
        <b-container>
            <b-row>
                <b-col cols="8">
                    <iframe class="vdo-hero" src="https://player.vimeo.com/video/354856987?autoplay=1&loop=1&autopause=0" width="640" height="360" frameborder="0" allow="autoplay;"></iframe>
                    <b-img class="img-hero" src="~assets/images/hero-bg.png" alt="bg"></b-img>
                </b-col>
                <b-col class="logo-countdown-button">
                    <b-img v-bind="mainProps" src="~assets/images/logo_white.png" alt="logo"></b-img>
                    <div class="countdown d-flex justify-content-center">
                            <div class="countdown-block pt-0 pb-0">
                                <h1>03</h1>
                                <p class="mb-0">months</p>
                            </div>
                            <div class="countdown-block pt-0 pb-0">
                                <h1>28</h1>
                                <p class="mb-0">days</p>
                            </div>
                            <div class="countdown-block pt-0 pb-0">
                                <h1>07</h1>
                                <p class="mb-0">hours</p>
                            </div>
                    </div>
                    <div class="button-hero mt-3">
                        <b-button class="button">GET TICKET NOW</b-button>
                        <b-button class="button">BOOTH RESERVATION</b-button>
                        <b-button class="button">IHSATEC</b-button>
                    </div>
                </b-col>
            </b-row>
        </b-container>
    </div>
</template>

<script>
export default {
    data() {
        return {
            mainProps : {
                fluid: true
            }
        }
    }
}
</script>
<style scoped>
    .vdo-hero {
        box-shadow: 20px -20px #D6AD00;
        margin-top: 6rem;
    }
    .button-hero {
        display: flex;
        flex-direction: column;
    }
    .button-hero .button {
        margin-bottom: 1rem;
        background-color: white;
        color: #0F051A;
        border-radius: 30px;
    }
    .logo-countdown-button {
        margin-top: 10rem;
    }
    .countdown .countdown-block {
        border-right: 1px white solid;
        padding: 1rem;
    }
    .img-hero {
        margin-top: -10rem;
        width: 90%;
    }
    h1 {
        font-size: 3.5rem !important;
    }

</style>

