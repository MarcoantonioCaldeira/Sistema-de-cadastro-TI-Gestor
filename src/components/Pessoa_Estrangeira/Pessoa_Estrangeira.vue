<template> 
    <div id="Area_Pessoa_Estrangeira" v-on:click="pessoa_estrangeira">
        <router-link to="Cadastro_pt_1_P_Estrangeira"><h2 class="h2_p_estrangeira">Pessoa Estrangeira</h2></router-link>
    </div>
</template>

<script>
export default {
    name: 'Pessoa_Estrangeira',

    methods: {
      Cadastro_Informacoes(){
            axios({
               method: 'post',
               url: 'localhost:9000/clientes',
               data: {
                pessoa_estrangeira: 2,
            }
        })
      }
   }
}
</script>
<style src="./estilo_inicio_p_estrangeira.scss"  lang="scss">

</style>
