<template>
    <section id="producto-imagen">
        <div class="img-principal"> 
            <img v-bind:src="fotos[0]" alt="Tv LG">
        </div>
    
        <div class="img-secundaria">
            <a @click="cambiarFoto(1)"><img  v-bind:src="fotos[1]" alt="Tv LG"></a>
            <a @click="cambiarFoto(2)"><img  v-bind:src="fotos[2]" alt="Tv LG"></a>
            <a @click="cambiarFoto(3)"><img  v-bind:src="fotos[3]" alt="Tv LG"></a>
            <a @click="cambiarFoto(4)"><img  v-bind:src="fotos[4]" alt="Tv LG"></a>
            <a @click="cambiarFoto(5)"><img  v-bind:src="fotos[5]" alt="Tv LG"></a>
        </div>
    </section>    
</template>

<script>
    export default {
        Name: 'ProductoImagen',
        data () {
            return {
                fotos: [
                        require ('../assets/e1.jpg'),
                        require ('../assets/e1.jpg'),
                        require ('../assets/e2.jpg'),
                        require ('../assets/e3.jpg'),
                        require ('../assets/e4.jpg'),
                        require ('../assets/e5.jpg')
                    ]
            }
        },
        methods: {
            cambiarFoto(id) {
                console.log("imagen " + id + " - " + this.fotos[id]);
                this.fotos[0]=this.fotos[id];
                console.log("imagen " + this.fotos[0] );
            }
        }

    }
</script>

<style>
    #producto-imagen {
        border-radius: 25px;
        padding: 1rem;
        padding-right: 6rem;
        margin: 1rem;
        margin-top: -20.3rem;
        /*background-color: navy;*/
    }

    .img-principal img{
        width: 100%;
    }

    .img-secundaria {
        display: flex;
        justify-content: space-between;
        align-items: flex-start;
    }

    .img-secundaria img {
        width: 100px;
        border: 2px solid #000000; 
    }
</style>