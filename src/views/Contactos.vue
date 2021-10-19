<template>
    <div class="contac">
        <h2>{{texto}}</h2>
        <div>
            <b-tabs content-class="mt-3" align="center">
                <b-tab title="Dudas acerca del sistema" active><p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Error temporibus facilis aut quam, cum incidunt ipsa corrupti id culpa ea vel distinctio voluptatem dolorem dolor voluptas at ut placeat cupiditate.</p></b-tab>
                <b-tab title="Quiero publicar y no sé como"><p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Vero ipsa non numquam tempora impedit laboriosam ipsam laborum alias nisi culpa, eveniet et quis officia sunt quam nostrum maiores suscipit consectetur?</p></b-tab>
                <b-tab title="Denuciar un problema"><p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Culpa sed ad corporis enim doloremque unde libero earum aspernatur nam! Rerum incidunt officiis velit eos minus vero fuga atque. Magni, debitis!</p></b-tab>

            </b-tabs>
        </div>
        <div class="container-xl">
            <div class="justify-content-center">
                 <b-form-group 
                    id="fieldset-horizontal"
                    label-cols-sm="4"
                    label-cols-lg="3"
                    content-cols-sm
                    content-cols-lg="7"
                    label="Nombre y Apellido"
                    label-for="input-horizontal"
                    >
                    <b-form-input id="input-horizontal"></b-form-input>
                </b-form-group>
                <b-form-group 
                    id="fieldset-horizontal"
                    label-cols-sm="4"
                    label-cols-lg="3"
                    content-cols-sm
                    content-cols-lg="7"
                    label="Telefono"
                    label-for="input-horizontal"
                    >
                    <b-form-input id="input-horizontal"></b-form-input>
                </b-form-group>
                <b-form-group 
                    id="fieldset-horizontal"
                    label-cols-sm="4"
                    label-cols-lg="3"
                    content-cols-sm
                    content-cols-lg="7"
                    label="Email    "
                    label-for="input-horizontal"
                    >
                    <b-form-input id="input-horizontal"></b-form-input>
                </b-form-group>
               <b-container fluid>           
                <b-row class="mt-2">
                    <b-col sm="2">
                    <label for="textarea-default">Consulta:</label>
                    </b-col>
                    <b-col sm="10">
                    <b-form-textarea
                        id="textarea-default"
                        placeholder="Consulta*"
                    ></b-form-textarea>
                    </b-col>
                    
                </b-row>
                <b-button type="submit" variant="primary" class="mt-3">Enviar</b-button>
                </b-container>
                
                
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Contact',
  props: {
    msg: String
  },
  data(){
    return{
      texto: "¿En qué podemos ayudarte?"
    }
  }
}
</script>