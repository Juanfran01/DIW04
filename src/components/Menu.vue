<template>
<section id="menu-principal">
    <div class="container">
        <nav>
            <ul>
                <li><a href="#">INICIO</a></li>
                <li><a href="#">ORDENADORES</a></li>
                <li><a href="#">SMART TV</a></li>
                <li><a href="#">MÓVILES</a></li>
                <li><a href="#">REPARACIONES</a></li>
            </ul>
        </nav>
    </div>
</section>
  
</template>

<script>
    export default {

    }
</script>

<style>

    section#menu-principal {
        background: gray;
        padding: 1rem;
    }

    section#menu-principal .container {
        display: flex;
        justify-content: space-between;
    }

    section#menu-principal .container nav ul {
        display:flex;
        list-style: none;
        padding: 0;
        margin: 0rem 1rem;
    }

    section#menu-principal .container nav ul li a {
        background-color:  gray;
        text-decoration: none;
        color:white;
        font-weight: 700;
        padding-left: 1rem;
        padding-right: 1rem;
    }

    section#menu-principal .container nav ul li a:hover{
        text-decoration: none;
        color: #F09D15;
        font-weight: 700;
        padding: 1rem;
    }

</style>