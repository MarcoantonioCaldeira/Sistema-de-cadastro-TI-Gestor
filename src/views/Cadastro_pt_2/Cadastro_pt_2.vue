<template>
  <div id="etapas">
    <etapas_info_endereco />
  </div>
    <div id="corpo_info_endereco">
      <h1 class="h1_info_endereco">Informações de endereço</h1>
      <Informacoes_Endereco />
    </div>
    <Footer />  

</template>


<script>

import Footer from '@/components/Footer.vue'
import Informacoes_Endereco from '@/components/informacoes_de_Endereco.vue'
import etapas_info_endereco from '@/components/etapas_info_endereco.vue';

export default {
  name: 'Cadastro_pt_2',
  components: {
    Informacoes_Endereco,
    etapas_info_endereco,
    Footer
  }
}
</script>
<style  src="./estilo.scss"  lang="scss">
</style>
