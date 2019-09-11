<template>
    <div class="comingsoon">
        <b-container fluid>
            <b-img class="img-hero" src="~assets/images/logo_white.png" alt="logo"></b-img>
            <countdown :time="2 * 24 * 60 * 60 * 1000">
                <template slot-scope="props">Time Remaining：{{ props.days }} days, {{ props.hours }} hours, {{ props.minutes }} minutes, {{ props.seconds }} seconds.</template>
            </countdown>
        </b-container>
    </div>
</template>


<script>
import Vue from 'vue';
import VueCountdown from '@chenfengyuan/vue-countdown';

export default {
    mounted() {
        this.$refs.countdown.start();
     },
    components: {
        VueCountdown
    }
    
}
</script>


<style scoped>
    .img-hero{
        width: 100%;
    }
    .comingsoon {
        z-index: 10000;
    }
</style>
