<template>
  <div class="container">
    <Hero />
    <News />
    <Agenda />
  </div>
</template>

<script>
import Hero from '~/components/Hero/Hero'
import News from '~/components/News/News'
import Agenda from '~/components/Agenda/Agenda'

export default {
  components: {
    Hero,
    News,
    Agenda
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
