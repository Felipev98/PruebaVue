<template>
  <section class="seccion" id="empleo">
            <div class="container">
                <div class="row">
                    <div class="col-xl-6 col-empleo">
                <Sections titulo="Búsqueda de empleo" contenido="La búsqueda de empleo en una economía incierta es bastante difícil. Agregue los temores por el coronavirus, las cuarentenas domiciliarias y la paralización en las contrataciones en muchas compañías.Millones de personas están compitiendo repentinamente por un grupo reducido de empleos, con más de 3.8 millones de trabajadores despedidos que solicitaron beneficios de desempleo solo la semana pasada, la cifra se ha elevado a 30.3 millones en las últimas seis semanas. "/>
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
import Sections from '@/components/SectionsComponents/Sections.vue'
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
      font-family: 'GardeGothic-Bold';

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
/* Versión Tablet */
@media screen and (min-width:701px) and (max-width:1023px){
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
        left: 12rem;
    }
}
@media screen and (min-width:1023px) and (max-width:1024px){
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
        left: 19rem;
    }
}
/* Final MediaQueries */
</style>