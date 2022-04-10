<template>
  <div>
    <HomeView />
    <PublicarVagas />
  </div>
</template>

<script>
import HomeView from '../views/HomeView.vue'
import PublicarVagas from '../views/PublicarVagas.vue'

 export default {
    name: 'ContentSite',
    components: {
      HomeView,
      PublicarVagas
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

</style>
