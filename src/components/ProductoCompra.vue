<template>
  <section id="producto-compra">
    <h1>
        LG OLED65C14LB 65"<br>
        OLED Ultra HD 4K HDR10 Pro
    </h1>
      
      <h2>1904,14€ <span class="iva">sin IVA: 1844,59€</span></h2>

      <div class="caja-compra">
            <button class="btn" @click="cambiarContador('-1')" type="button" name="button">-</button>
            <input class="cantidad" type="text" name="name" :value="contador">
            <button class="btn" @click="cambiarContador('1')" type="button" name="button">+</button>
      </div>
      <br>

        <button class="boton"><span class="material-icons">shopping_basket</span>AÑADIR CARRITO</button>
    
  </section>
</template>

<script>
    export default {
    Name: 'ProductoCompra',
        data () {
            return {
                contador: 1
            }
        },
        methods: {
            cambiarContador(num) {
                this.contador += +num;
                if (!isNaN(this.contador) && (this.contador < 0)) {
                this.contador = 0
                }
            }

        }
    }
</script>


<style>

    section#producto-compra{
        justify-content: flex-end;
        margin: 1rem;
        margin-top: 7rem;
    }

    h1 {
        font-size: 2.2rem;
    }

	h2 {
        font-size:1.7rem;
        color: #3A3F49;
    }

	span.iva {
        font-size: 1rem;
        font-weight: normal;
        color: #282828;
    }

	.caja-compra {
        height: 2rem;
        display: flex;
    }

    .cantidad {
        text-align: center;
        width: 3rem;
        font-size: 1.5rem;
        border: 1px solid #3A3F49;
    }

	.btn {
        border: 1px solid #3A3F49;
        width: 1.8rem;
    }

</style>