<template>
  <div>
    <TheHeader />
    <main class="main-content">
      <nuxt />
    </main>
  </div>
</template>


<script>
  import Vue from 'vue'
  import BootstrapVue from 'bootstrap-vue'
  import TheHeader from '@/components/TheHeader/TheHeader'


  Vue.use(BootstrapVue)

  export default {
    components: {
      TheHeader
    }
  }
</script>


<style>
  * {
    box-sizing: border-box;
  }
  body {
    font-family: 'Oswald', sans-serif;
    background-color: #210837;
    color: white;
  }
  .main-content {
    margin-left: 10rem;
    margin-right: 3rem;
  }
</style>
