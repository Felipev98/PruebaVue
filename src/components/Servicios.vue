<template>
  <section class="servicios">
      <div class="container">
          <div class="row">
                <Sections titulo="Servicios" contenido="demdemdeomdeomdeomdoemdomed"/>
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
import Sections from '@/components/Sections.vue'
export default {
    data() {
        return {
            servicios:{
                servicio1:{
                    imagen:'bombillo.svg',
                    titulo:'Gestión de talento humano',
                    contenido:'Connection to the API of YouTube to access videos from “Gentleman Programming.”',
                },
                servicio2:{
                    imagen:'search.svg',
                    titulo:'Búsqueda de empleo',
                    contenido:'Connection to the API of YouTube to access videos from “Gentleman Programming.”',
                },
                servicio3:{
                    imagen:'people.svg',
                    titulo:'Asesoría estratégica empresarial',
                    contenido:'Connection to the API of YouTube to access videos from “Gentleman Programming.”',
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
.servicios{
    height: auto;
}

.imagen-card{
    text-align: center;
}
.imagen-card img{
    width: 5rem;
}
.card-title{
    text-align: center;
    color: #ffff;
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
@media screen and (max-width:700px){
    .cards{
        margin: auto;
    }
    .servicios{
        margin-top: 2rem;
    }
}

/* Final Sección MediaQueries */
</style>