<template>
  <a-layout class="layout-demo">
    <!-- <SideBar></SideBar> -->
    <a-layout>
      <HeaderBar></HeaderBar>
      <a-layout>
        <a-breadcrumb :style="{ margin: '16px 0' }">
          <a-breadcrumb-item>Home</a-breadcrumb-item>
          <a-breadcrumb-item>List</a-breadcrumb-item>
          <a-breadcrumb-item>App</a-breadcrumb-item>
        </a-breadcrumb>
      </a-layout>
    </a-layout>
  </a-layout>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import HeaderBar from './components/HeaderBar.vue'
// import SideBar from './components/SideBar.vue'

export default {
  name: 'App',
  components: {
    HeaderBar
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: var(--color-fill-2);
}
.layout-demo {
  height:100vh;
}
</style>
