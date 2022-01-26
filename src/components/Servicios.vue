<template>
  <section class="seccion" id="servicios">
      <div class="container">
          <div class="row">
                <Sections titulo="Servicios" contenido="Nuestros servicios se diferencian por la atención personalizada que le brindamos a cada uno de nuestros clientes, nos enfocamos en cumplir los objetivos y dar más allá de los resultados esperados."/>
                <div v-for="servicio in servicios" :key="servicio.id" class="col-xl-4">
                <div class="cards" style="width: 18rem; margin-top: 1rem;">
                <div class="imagen-card">
                <img class="card-img-top" :src="require(`../assets/${servicio.imagen}`)" alt="Card image cap">
                </div>
                <div class="card-body">
              <h5 class="card-title card-t-2">{{servicio.titulo}}</h5>
              <p class="card-title">{{servicio.contenido}}</p>
              </div>
                </div>
                </div>
          </div>
      </div>
  </section>
</template>

<script>
import Sections from '@/components/SectionsComponents/Sections.vue'
export default {
    data() {
        return {
            servicios:{
                servicio1:{
                    imagen:'bombillo.png',
                    titulo:'Gestión de talento humano',
                    contenido:'El objetivo de la gestión de Recursos Humanos es que la empresa cuente con el personal más apto y calificado, que sean bien remunerados',
                },
                servicio2:{
                    imagen:'search.png',
                    titulo:'Búsqueda de empleo en cualquier lugar',
                    contenido:'Te ayudamos a conectar con empresas que buscan personal calificado y que estén dispuestas a contratar a los mejores trabajadores del mundo',
                },
                servicio3:{
                    imagen:'people.png',
                    titulo:'Asesoría estratégica empresarial',
                    contenido:'Consiste en aprovechar las novedades en el entorno empresarial para beneficiar a la empresa,Para obtener los mejores beneficios en la empresa',
                },
            }
        }
    },
components:{
    Sections
    },
}
</script>

<style>
.imagen-card{
    text-align: center;
}
.imagen-card img{
    width: 9rem;
}
.card-title{
    text-align: center;
    color: #ffff;
}
.card-title:first-child{
      font-family: 'GardeGothic-Bold';

}
.cards{
    padding:1rem;
    border-radius: 0.8rem;
    background-color: #43506A;
    position: relative;
    display: flex;
    flex-direction: column;
    min-width: 0;
    word-wrap: break-word;
    background-clip: border-box;
    border: 1px solid rgba(0, 0, 0, 0.125);
    border-radius: 0.8rem;
}

/* Inicio sección MediaQueries */
@media screen and (max-width:1024px){
    .cards{
        margin: auto;
    }
    .servicios{
        margin-top: 2rem;
    }
}

/* Final Sección MediaQueries */
</style>