<template>
  <section id="breadcrumb">
      <a class="inicio" href="#"> Inicio </a> <p>></p>
      <a href="#">Smart TV </a> <p>></p>
      <a class="seleccionado" href="#">TV LG</a> 
  </section>
</template>

<script>
export default {

}
</script>

<style>

    section#breadcrumb {
        display: flex;
        padding: 1rem;
    }

    section#breadcrumb p, 
    section#breadcrumb a, 
    section#breadcrumb a:hover, 
    section#breadcrumb a:visited{
        text-decoration: none;
        font-size: 1rem;
        margin-top: 2rem;
        margin-left: 1rem;
        margin-right: 1rem;
        color: #3A3F49;
    }

    section#breadcrumb a.seleccionado {
        font-weight: 900;
    }

    section#breadcrumb {
        color: #3A3F49;
    }

</style>