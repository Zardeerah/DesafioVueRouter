<template lang="">
  <!-- Sección de cartas de productos -->
  <section class="container" id="productos">
    <h1 class="text-center">Nuestros Productos</h1>
    <div class="row">
      <div class="col-sm-4 col-12 px-5 mb-4">
        <div class="card">
          <img src="../assets/img/colaciones.jpg" class="card-img-top" alt="Imagen de colaciones" />
          <div class="card-body">
            <h5 class="card-title fw-bold">Colaciones</h5>
            <p class="card-text">
              Some quick example text to build on the card title and make up the bulk of the card's content.
            </p>
          </div>
          <ul class="list-group list-group-flush">
            <li class="list-group-item">Dapibus ac facilisis in</li>
            <li class="list-group-item">Vestibulum at eros</li>
          </ul>
          <div class="card-body">
            <a href="#" class="btn btn-primary">Ver más</a>
            <a href="#" class="btn btn-success">Comprar</a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Card'
}
</script>

<style scoped lang="css">
#productos {
  margin-top: 2rem;
}

.card-img-top {
  height: 250px;
  object-fit: cover;
}

.card-body {
  padding: 1.5rem;
}

.card-title {
  font-size: 1.25rem;
}

.btn-vermas {
  background-color: #007bff;
  color: white;
  border-radius: 5px;
  padding: 0.5rem 1rem;
  text-decoration: none;
}

.btn-vermas:hover {
  background-color: #0056b3;
}

.btn-comprar {
  background-color: #28a745;
  color: white;
  border-radius: 5px;
  padding: 0.5rem 1rem;
  text-decoration: none;
}

.btn-comprar:hover {
  background-color: #218838;
}

.card-body .btn {
  margin-right: 10px;
  display: inline-block;
}
</style>

