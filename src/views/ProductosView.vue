<script>
import Card from "@/components/Card.vue";

export default {
  name: 'DetalleProducto',
  props: {
    nombre: String,
    descripcion: String,
    precio: Number,
    cantidad: Number
  }
}
</script>
<template>
    <section class="container text-center" id="productos">
      <h1>Detalle del Producto</h1>
      <div class="row justify-content-center">
        <div class="col-md-6 col-lg-4 col-12 px-3 mb-4">
          <div class="card">
            <img 
              :src="require('@/assets/img/colaciones.jpg')" 
              class="card-img-top" 
              alt="Imagen de colaciones" 
            />
            <div class="card-body">
              <h5 class="card-title fw-bold">{{ nombre }}</h5>
              <p class="card-text">{{ descripcion }}</p>
            </div>
            <ul class="list-group list-group-flush">
              <li class="list-group-item">Precio: ${{ precio }}</li>
              <li class="list-group-item">Cantidad: {{ cantidad }}</li>
            </ul>
            <div class="card-body d-flex justify-content-between">
              <router-link class="btn btn-primary" to="/">Ver más</router-link>
              <router-link class="btn btn-success" :to="{ name: 'contacto' }">Comprar</router-link>
            </div>
          </div>
        </div>
        <router-link class="btn btn-outline-secondary mt-3" to="/">Volver al Inicio</router-link>
      </div>
    </section>
  </template>
  
  
  
  <style scoped>
  #productos {
    margin-top: 2rem;
  }
  
  .card {
    border-radius: 10px;
    overflow: hidden;
  }
  
  .card-body {
    padding: 1.5rem;
  }
  
  .card-img-top {
    height: 250px;
    object-fit: cover;
  }
  
  h1 {
    margin-bottom: 2rem;
  }
  
  .list-group-item {
    font-size: 1.1rem;
  }
  
  .btn {
    width: 45%;
  }
  
  @media (max-width: 768px) {
    .btn {
      width: 100%;
      margin-bottom: 1rem;
    }
  }
  </style>