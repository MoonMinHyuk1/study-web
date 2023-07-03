<template>
  <div class='app'>
    <main-header></main-header>
    <main-nav></main-nav>
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </nav>
    <router-view/>
    <main-footer></main-footer>
  </div>
</template>

<script lang="ts">
import MainHeader from './components/common/Header.vue'
import MainFooter from './components/common/Footer.vue'
import MainNav from './components/common/Nav.vue'
export default {
  components: {
    MainHeader,
    MainFooter,
    MainNav
  }
}
</script>

<style lang="stylus">
#app
  font-family Avenir, Helvetica, Arial, sans-serif
  -webkit-font-smoothing antialiased
  -moz-osx-font-smoothing grayscale
  text-align center
  color #2c3e50
  margin-top 60px
</style>
