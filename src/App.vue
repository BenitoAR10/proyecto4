<template>
  <div id="app" class="text-center">
    <b-navbar toggleable="md" type="dark" variant="info">
      <b-navbar-brand href="#">Empresa Inmobiliaria</b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav>
            <b-nav-item :to="{name:'Home'}">Home</b-nav-item>
            <b-nav-item :to="{name:'About'}">Ofertas de casas</b-nav-item>
            <b-nav-item :to="{name:'Clientes'}">Requerimientos de clientes</b-nav-item>
            <b-nav-item :to="{name:'Contactos'}">Contactos</b-nav-item>
          </b-navbar-nav>
        </b-collapse>
    </b-navbar>  
    <router-view/>
    <p class="fs-5 px-3 pt-3">Empresa Inmobiliaria &copy; Realizado por Amir Rojas 2021</p>
  </div>
  
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
