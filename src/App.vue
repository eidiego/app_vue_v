<template>
  <div>

    <Top />
    <Content />

  </div>
</template>

<script>
import Content from './components/layouts/ContentSite.vue'
import Top from './components/layouts/TopSite.vue'

export default {
  name: 'App',
  components: {
    Content,
    Top
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
  margin-top: 60px;
}
</style>
