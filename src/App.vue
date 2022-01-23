<template>

  <div>
    <Cabecera/>
    <Menu/>

    <div class="container">
      <Ruta-breadcrumb/>
    </div>
    
    <div class="columna-uno">
      <ProductoCompra/>
    </div>

    <div class="columna-dos">
      <ProductoImagen/>
    </div>
    
    <div class="container">
      <ProductoDescripcion/>
    </div>  
    
    <div class="footer">
      <Pie/>
    </div>
  </div>

</template>

<script>
import Cabecera from './components/Cabecera.vue'
import Menu from './components/Menu.vue'
import RutaBreadcrumb from './components/RutaBreadcrumb.vue'
import ProductoCompra from './components/ProductoCompra.vue'
import ProductoImagen from './components/ProductoImagen.vue'
import ProductoDescripcion from './components/ProductoDescripcion.vue'
import Pie from './components/Pie.vue'


export default {
  name: 'App',
  components: {
    Cabecera,
    Menu,
    RutaBreadcrumb,
    ProductoCompra,
    ProductoImagen,
    ProductoDescripcion,
    Pie
  }
}
</script>



<!-- Estilos -->

<style>

  body{
    margin: 0px;
    padding: 0px;
    display: flex;
    flex-direction: column;
  }

  .container {
      max-width: 1400px;
      margin: auto;
  }

  .columna-uno {
    display: flex;
    margin: 1rem;
    justify-content: flex-end;
    flex-wrap: wrap;
  }

  .columna-dos {
    display: flex;
    margin: 1rem;
    justify-content: flex-start;
    flex-wrap: wrap;
  }

  .boton {
    background-color: #3A3F49;
    font-size: 1.2rem;
    font-weight: 700;
    color: white;
    padding: 0.7rem 1.2rem;
    cursor: pointer;
    border: none;
  }

  .boton:hover {
    color: orange;
    background-color: black;
  }

</style>
