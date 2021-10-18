<template>
  <div id="app" class="text-center">
    <b-navbar toggleable="md" type="dark" variant="info">
      <b-navbar-brand href="#">Empresa Inmobiliaria</b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav>
            <b-nav-item :to="{name:'home'}">Home</b-nav-item>
            <b-nav-item :to="{name:'MiComponente'}">Ofertas de casas</b-nav-item>
            <b-nav-item :to="{name:'MiComponente'}">Requerimientos de clientes</b-nav-item>
            <b-nav-item :to="{name:'HelloWord'}">Contactos</b-nav-item>
          </b-navbar-nav>
        </b-collapse>
    </b-navbar>

    

    <HelloWorld msg="Bienvenido a"/>
    <MiComponente></MiComponente>
    <Info></Info>
    <Ofertas></Ofertas>
    <Footer></Footer>
    
    
    
  </div>
</template>

<script>

import HelloWorld from './components/HelloWorld.vue'
import MiComponente from './components/MiComponente.vue'
import Info from './components/Info.vue'
import Footer from './components/Footer.vue'
import Ofertas from './components/Ofertas.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    MiComponente,
    Info,
    Footer,
    Ofertas
  }
}

</script>


