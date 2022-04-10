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
 
}
</style>
