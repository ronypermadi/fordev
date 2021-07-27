<template>
  <div class="wrapper">
    <Header/>
    <Navbar/>
    <!-- content -->
    <div class="page-wrapper">
      <div class="container-xl">
        <div class="mt-2 mb-2" id="app">
          <router-view />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: rgb(218, 214, 214);
}
</style>

<script>
// @ is an alias to /src
import Navbar from '@/components/Navbar.vue'
import Header from '@/components/Header.vue'

export default {
  name: 'AppComponent',
  components: {
    Navbar,Header
  }
}
</script>