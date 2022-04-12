<template>
  <div class="container py-4">
    <div class="row">
      <div class="col">
       
       <pesquisar-vaga></pesquisar-vaga>

      </div>
    </div>

    <div class="row mt-5">
        <div class="col-4">
            <indicador-site></indicador-site> 
        </div>
        
         <div class="col-4">
            <indicador-site></indicador-site> 
        </div>

         <div class="col-4">
            <indicador-site></indicador-site> 
        </div>
    </div>
  </div>
</template>

<script>

import PesquisarVaga from '@/components/comuns/PesquisarVaga.vue'
import IndicadorSite from '@/components/comuns/IndicadorSite.vue'

export default {
  name: 'HomeView',
  components: {
    PesquisarVaga,
    IndicadorSite
  } 
}
</script>

<style scoped></style>