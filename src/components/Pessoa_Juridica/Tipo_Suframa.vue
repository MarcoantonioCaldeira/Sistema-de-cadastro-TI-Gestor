<template>
        <h2 class="h2_suframa">Tipo <strong>SUFRAMA</strong>(Superintendência da<br>Zona Franca de Manaus)</h2>    
        <br>
        <select class="select" v-model="tipo_suframa">
            <option>ZFM(Zona Franca de Manaus)</option>
            <option>ALC(Área de Livre Comercio)</option>
            <option>Am. Ocid(Amazonia Ocidental)</option>
        </select>
        
        <br><label class="label_codigo_suframa">Codigo SUFRAMA:</label><input type="text" style="display: inline" class="input_suframa" v-model="codigo_suframa">
        
        <br><label class="label_num_inscricao">Numero de inscrição municipal: </label><input type="text" style="display: inline" class="input_inscricao" v-model="numero_inscricao_municipal">
</template>



<script>
import axios from 'axios';

export default{
    name: 'Tipo_Suframa',

    methods: {
      Cadastro_Informacoes(){
            axios({
               method: 'post',
               url: 'localhost:9000/clientes',
               data: {
                  tipo_suframa: "",
                  codigo_suframa: "",
                  numero_inscricao_municipal: ""
            }
         })
      }
   }
}
</script>