<template>
  <div class="container">
    <div class="row">
        <div class="col-12" id="hero">
            <div class="texto text-center">
                <h2>{{titulo}}</h2>
             <router-link to="/login" ><button class="boton-hero">{{boton}}</button></router-link>   
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    data() {
        return {
            titulo: 'SOLO 2 MINUTOS TE SEPARAN DE ENCONTRAR TU EMPLEO IDEAL',
            boton: 'Quiero entrar'
        }
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


/* Final Sección MediaQueries */
</style>