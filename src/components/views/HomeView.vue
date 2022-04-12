<template>
  <div class="container py-4">
    <div class="row">
      <div class="col">
       
       <pesquisar-vaga></pesquisar-vaga>

      </div>
    </div>

    <div class="row mt-5">s
        <div class="col-3">
            <indicador-site titulo="Vagas abertas" indicador="100"></indicador-site> 
        </div>

         <div class="col-3">
            <indicador-site titulo="Profissionais cadastrados" indicador="225"></indicador-site> 
        </div>

         <div class="col-3">
            <indicador-site titulo="Visitantes online" indicador="120"></indicador-site> 
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