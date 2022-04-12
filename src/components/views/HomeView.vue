<template>
  <div class="container py-4">
    <div class="row">
      <div class="col">
       
       <pesquisar-vaga></pesquisar-vaga>

      </div>
    </div>


    <div class="row mt-5">
      <div class="col">
          <vagas-component></vagas-component>
      </div>  
    </div>


    <div class="row mt-5">
        <div class="col-3">
            <indicador-site titulo="Vagas abertas" indicador="100" bg="bg-dark" color="text-white"></indicador-site> 
        </div>

         <div class="col-3">
            <indicador-site titulo="Profissionais cadastrados" indicador="225" bg="bg-dark" color="text-white"></indicador-site> 
        </div>

         <div class="col-3">
            <indicador-site titulo="Visitantes online" :indicador="usuariosOnline" bg="bg-light" color="text-dark"></indicador-site> 
        </div>
        
    </div>
  </div>
</template>

<script>

import PesquisarVaga from '@/components/comuns/PesquisarVaga.vue'
import IndicadorSite from '@/components/comuns/IndicadorSite.vue'
import VagasComponent from '@/components/comuns/Vagas.vue'

export default {
  name: 'HomeView',
  components: {
    PesquisarVaga,
    IndicadorSite,
    VagasComponent
  },
  data: () => ({
    usuariosOnline: 0
  }),
  methods: {
    getUsuariosOnline() {
     this.usuariosOnline = Math.floor(Math.random() * 101)
    }
  },
  created() {
    setInterval(this.getUsuariosOnline, 1000)
  }
}
</script>

<style scoped></style>