<template>
  <div id="app">
    <AppTitle />
    <HeroJumbo />
    <div>
      <img :src='imgUrl' alt="img">
      <div v-for="(item, index) in test" :key="index">
        {{ item }}
        <FirstComponent />
      </div>
    </div>
  </div>
</template>

<script>
import AppTitle from './components/AppTitle.vue'
import HeroJumbo from './components/HeroJumbo.vue'
import FirstComponent from './components/FirstComponent.vue'

export default {
  name: 'App',
  components: {
    AppTitle,
    HeroJumbo,
    FirstComponent,
  },
  data() {
    return {
      test: [1, 2, 1, 5, 4],
      imgUrl: './assets/logo.png'
    }
  }
}
</script>

<style lang="scss">
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
