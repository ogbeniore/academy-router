<template>
  <div id="app">
    <Navbar />
    <div class="row d-flex">
      <Sidebar />
      <router-view/>
    </div>
    <footer>
      <p>copyright &copy; 2019</p>
    </footer>
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'
import Sidebar from '@/components/Sidebar.vue'
export default {
  name: 'App',
  components: {
    Navbar,
    Sidebar
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
.red-border {
  border:  2px solid red;
}
.green-border {
  border:  2px solid green;
}
</style>
