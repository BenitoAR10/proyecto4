<template>
  <div class="container-xl">
      <div class="justify-content-center">
        <b-form @submit="onSubmit" @reset="onReset" v-if="show">
        <b-form-group
            id="input-group-1"
            label="Email:"
            label-for="input-1"
        >
            <b-form-input
            id="input-1"
            v-model="form.email"
            type="email"
            placeholder="Email"
            required
            ></b-form-input>
        </b-form-group>

        <b-form-group id="input-group-2" label="Nombre completo:" label-for="input-2">
            <b-form-input
            id="input-2"
            v-model="form.name"
            placeholder="Nombre"
            required
            ></b-form-input>
        </b-form-group>

        <b-form-group id="input-group-3" label="Telefono:" label-for="input-3">
            <b-form-input
            id="input-3"
            v-model="form.phone"
            placeholder="Telefono"
            required
            ></b-form-input>
        </b-form-group>

         <b-form-textarea
            id="textarea"
            v-model="text"
            placeholder="Información sobre su inmueble"
            rows="3"
            max-rows="6"
        ></b-form-textarea>

      <b-form-group id="input-group-5" label="Fotos:" label-for="input-5">
        <b-form-file
        v-model="file1"
        :state="Boolean(file1)"
        placeholder="Subir fotografias del inmueble"
        drop-placeholder="Drop file here..."
        ></b-form-file>
      </b-form-group>
        
        

        <b-form-group id="input-group-4" label="Precio:" label-for="input-4">
            <b-form-input
            id="input-4"
            v-model="form.price"
            placeholder="Precio"
            required
            ></b-form-input>
        </b-form-group>

        <b-form-group id="input-group-4" v-slot="{ ariaDescribedby }">
            <b-form-checkbox-group
            v-model="form.checked"
            id="checkboxes-4"
            :aria-describedby="ariaDescribedby"
            >
            <b-form-checkbox value="me">Aceptar terminos y condiciones</b-form-checkbox>
          
            </b-form-checkbox-group>
        </b-form-group>

        <b-button type="submit" variant="primary">Submit</b-button>
        <b-button type="reset" variant="danger">Reset</b-button>
        </b-form>
        <b-card class="mt-3" header="Form Data Result">
        <pre class="m-0">{{ form }}</pre>
        </b-card>
        </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        form: {
          email: '',
          name: '',
          phone: ''
        },
        
        show: true
      }
    },
    methods: {
      onSubmit(event) {
        event.preventDefault()
        alert(JSON.stringify(this.form))
      },
      onReset(event) {
        event.preventDefault()
       
        this.form.email = ''
        this.form.name = ''
        this.form.phone = null
       
        this.show = false
        this.$nextTick(() => {
          this.show = true
        })
      }
    }
  }
</script>