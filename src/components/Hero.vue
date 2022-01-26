<template>
  <div class="container">
    <div class="row">
        <div class="col-12" id="hero">
            <div class="texto text-center">
                <h2>{{titulo}}</h2>
             <a href="#empleo" ><button class="boton-hero">{{boton}}</button></a>   
            </div>
        </div>
    </div>
</div>
</template>
<script>
import gsap from 'gsap'
export default {
    data() {
        return {
            titulo: 'SOLO 2 MINUTOS TE SEPARAN DE ENCONTRAR TU EMPLEO IDEAL',
            boton: 'Quiero entrar'
        }
    },
    mounted() {
        gsap.from('.texto', {
            duration: 1.5,
            opacity: 0,
            y: -100,
        })
    },
}
</script>
<style>
#hero{
     height: 85vh;
     display: flex;
     align-items:center;
     justify-content: center;
 }
 .texto p{
     width: 40%;
     margin: auto;
     color: #D8D6D6;
 }
 .texto h2{
     color: #BFBFBF;
    font-size: 3.5rem;
      font-family: 'GardeGothic-Bold';
 }
 .boton-hero{
    margin-top: 1.2rem;
    border: none;
    padding: 0.8rem;
    width: 18%;
    background: #82DEBE;
    border-radius: 1.8rem;
    color: #ffff;
}
/* Inicio Sección MediaQueries */
@media screen and (max-width:700px){
    .texto h2{
        font-size: 1.5rem;
    }
    .boton-hero{
        width:60%;
    }
}

/* Versión tablet */

@media screen and (min-width:701px) and (max-width:1024px){
    .texto h2{
        font-size: 2.5rem;
    }
    .boton-hero{
        width:35%;
    }
    .titulo{
        text-align: center;
    }
}

/* Final Sección MediaQueries */
</style>