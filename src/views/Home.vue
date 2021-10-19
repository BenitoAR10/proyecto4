<template>
  <div class="home">
    <b-carousel
            id="carousel-fade"
            style="text-shadow: 0px 0px 2px #000"
            fade
            indicators
            img-width="700"
            img-height="250"
        >
            <b-carousel-slide
            caption="First slide"
            img-src="https://media.istockphoto.com/photos/home-with-blue-siding-and-stone-faade-on-base-of-home-picture-id1272128530?b=1&k=20&m=1272128530&s=170667a&w=0&h=k9lT5-DEmkmehDb-EKRHoP1-op2DTgz4ibiWGXmj7h8=" class="w-50 rounded"
            ></b-carousel-slide>
            <b-carousel-slide
            caption="Second Slide"
            img-src="https://images.unsplash.com/photo-1512917774080-9991f1c4c750?ixid=MnwxMjA3fDB8MHxzZWFyY2h8MXx8aG9tZXN8ZW58MHx8MHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" class="w-50 rounded" 
            ></b-carousel-slide>
            <b-carousel-slide
            caption="Third Slide"
            img-src="https://media.istockphoto.com/photos/colonial-style-house-picture-id1284097677?b=1&k=20&m=1284097677&s=170667a&w=0&h=1A7BkHG5OU4WCN7m22OOhvVmU21q4UsYVJPrS1kgcKI=" class="w-50 rounded"
        ></b-carousel-slide>
        </b-carousel>
     <h2>{{texto}}</h2>
    <div class="container-fluid">
        <div class="row">
            <div class="col-md-4">
                <b-card
                    title="Todas las propiedades"
                    img-src="https://images.unsplash.com/photo-1491357492920-d2979986a84e?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8Mnx8aG9tZXN8ZW58MHx8MHx8&auto=format&fit=crop&w=500&q=60"
                    img-alt="Image"
                    img-top
                    tag="article"
                    style="max-width: 20rem;"
                    class="ml-5"
                >
                    <b-card-text>
                    Con más de 20.000 propiedades publicadas, alcanzamos el 100% de ofertas inmobiliarias del país
                    </b-card-text>

                    <b-button href="#" variant="primary">Ver propiedades</b-button>
                </b-card>
            </div>
            <div class="col-md-4">
                <b-card
                    title="Alquiler/Venta de casas"
                    img-src="https://images.unsplash.com/photo-1600585154363-67eb9e2e2099?ixid=MnwxMjA3fDB8MHxzZWFyY2h8N3x8aG9tZXN8ZW58MHx8MHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60"
                    img-alt="Image"
                    img-top
                    tag="article"
                    style="max-width: 20rem;"
                    class="ml-5"
                >
                    <b-card-text>
                    Tenemos herramientas para que puedas tomar la mejor decisión basadas en datos
                    </b-card-text>

                    <b-button href="#" variant="primary">Más info</b-button>
                </b-card>
            </div>
             <div class="col-md-4">
                <b-card
                    title="Alquiler/Venta de departamentos"
                    img-src="https://images.unsplash.com/photo-1501183638710-841dd1904471?ixid=MnwxMjA3fDB8MHxzZWFyY2h8MTd8fGhvbWVzfGVufDB8fDB8fA%3D%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60"
                    img-alt="Image"
                    img-top
                    tag="article"
                    style="max-width: 20rem;"
                    class="ml-5"
                >
                    <b-card-text>
                    Tenemos herramientas para que puedas tomar la mejor decisión basadas en datos
                    </b-card-text>

                    <b-button href="#" variant="primary">Más info</b-button>
                </b-card>
            </div>
        </div>
        <div class="w-75 m-auto text-center" id="equipo">
            <h1 class="mb-5 fs-2">Equipo pequeño con <span class="text-primary"> resultados grandes</span></h1>
            
        </div>
    </div>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>
