<template>
  <div class="body">
    <NavBar />
    <SecOne />
    <SecTwo />
    <SecTre />
    <SecFour />
    <SecFive />
    <SecSix />
    <FooTer />
  </div>
</template>

<script>
import NavBar from './components/Navbar.vue'
import SecOne from './components/section1.vue'
import SecTwo from './components/section2.vue'
import SecTre from './components/section3.vue'
import SecFour from './components/section4.vue'
import SecFive from './components/section5.vue'
import SecSix from './components/section6.vue'
import FooTer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    SecOne,
    SecTwo,
    SecTre,
    SecFour,
    SecFive,
    SecSix,
    FooTer

  }
}
</script>

<style>
.body {
  margin: -8px;
  display: flex;
  flex-direction: column;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0px;
  padding: 0px;
  border: 0px;
}
</style>
