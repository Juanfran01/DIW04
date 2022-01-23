<template>

    <section id="cabecera">

        <div  class="logo">
            <img src="../assets/logo.png" alt="Logo de la empresa">
        </div>

        <div id="barra-navegar">
        </div>

        <div class="grupo-principal">
            <a class="registro" href="#">REGISTRO</a>
            <a class="login" href="#">INICIAR SESIÓN</a>
        </div>
    </section>

</template>

<script>
    export default {

    }
</script>

<!-- Estilos -->
<style>

    #cabecera{
        background-color: #3A3F49;
        padding: 0.5rem;
    }

    .logo img{
        align-items: stretch;
        max-width: 10%;
    }

    .grupo-principal{
        padding: 1.5rem;
        display: flex;
        justify-content: flex-end;
        align-content: flex-end;
        margin-top: -5rem;
    }

    .grupo-principal a{
        text-decoration: none;
        color: white;
        padding: 0.5rem;
        /*padding-left: 1rem;    */
    }

    .grupo-principal a:hover{
        color: orange;
        text-decoration: none;
    }

</style>