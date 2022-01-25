<template>
  <section class="empleo">
            <div class="container">
                <div class="row">
                    <div class="col-xl-6 col-empleo">
                <Sections titulo="Búsqueda de empleo" contenido="is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. "/>
                    </div>
                    <div class="col-xl-6">
                        <div class="imagen">
                            <img src="../assets/Empleo.png" alt="">
                        </div>
                        <div class="imagen-mensaje"></div>
                        <div class="mensaje">
                            <span class="text-imagen">{{nombre}}</span>
                            <span>{{mensaje}}</span>
                        </div>
                    </div>
                </div>
      </div>
  </section>
</template>

<script>
import Sections from '@/components/Sections.vue'
export default {
    name:'Empleo',
    data() {
        return {
            nombre:'Bruno Díaz',
            mensaje:'He conseguido mi primer empleo gracias a esta aplicación 😍😍😍😍',
        }
    },
    components:{
        Sections
    },
}
</script>

<style>
.empleo{
    height: auto;
    padding-top: 4rem;
}
.imagen img{
    width: 25rem;
}
.col-empleo{
    display: flex;
    align-items: center;
}
.mensaje{
  position: relative;
  padding: 1rem;
background: rgba(255, 255, 255, .7);
-webkit-backdrop-filter: blur(10px);
backdrop-filter: blur(10px);
  top: -8rem;
  left: -1rem;
  z-index: 99999;
  border-radius: 0.7rem;
  width: 20rem;
}
.text-imagen{
    display: block;
}
.imagen-mensaje{
width: 3rem;
  height: 3rem;
  border-radius: 50%;
  background-image: url('../assets/persona.png');
  background-size: cover;
  background-position: center;
  display: inline-block;
  position:relative;
  top:-6.5rem;
  border:1px solid green;
  z-index: 999999;
}

/* Inicio MediaQueries */
@media screen and (max-width:700px){
    .imagen{
        text-align: center;
    }
    .imagen img{
        width: 19rem;
    }
    .mensaje{
        margin: auto;
    }
    .imagen-mensaje{
        left: 2rem;
    }
}


/* Final MediaQueries */
</style>