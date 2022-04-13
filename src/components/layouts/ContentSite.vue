<template>
  <div>
     <div>
    <h1>{{titulo}}</h1>
    <button @click="atualizarComponente()">Atualizar</button>
    <button @click="conteudo = 'HomeView'">Home</button>
    <button @click="conteudo = 'publicar-vaga'">Publicar Vaga</button>
    <!-- renderizar de modo dinâmico os componentes home e publicar-vaga -->
    <!--<home></home>-->
    <!--<publicar-vaga></publicar-vaga>-->
    <keep-alive>
      <component :is="conteudo" />
    </keep-alive>
     </div>
  </div> 
 </template>

<script>
import HomeView from '../views/HomeView.vue'
import PublicarVaga from '../views/PublicarVaga.vue'

 export default {
    name: 'ContentSite',
    components: {
      HomeView,
      PublicarVaga
    },
    data: () => ({
    teste: 'O componente foi criado',
    titulo: 'Componente Conteudo',
    conteudo: 'HomeView'
  }),
     methods: {
        atualizarComponente() {
          this.titulo += '*'
    }
  },
 } 
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>

</style>
