<template>
  <div class="tarjeta-talento">
        <div class="numero">
            <h2>{{numero}}</h2>
        </div>
    <div class="titulo-numero">
        <span>{{titulopasos}}</span>
    </div>
    <div class="titulo-numero">
        <span>{{contenidopasos}}</span>
    </div>
</div>
</template>

<script>
export default {
    name: 'Pasos',
    props:{
        numero:{
            type:Number,
        },
        titulopasos:{
            type:String,
        },
        contenidopasos:{
            type:String,
        },
    },
    }
</script>

<style>
.tarjeta-talento{
    background: #3E4450;
    height: 13rem;
    padding: 1rem;
    border-radius: 0.9rem;
    margin-top: 1rem;
    color: #ffff;
}
.numero h2{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 3rem;
    height: 3rem;
    background: #82DEBE;
    border-radius: 50%;
    color: white;
}
/*  Inicio MediaQueries  */
@media screen and (max-width:700px){
    .numero h2{
        margin: auto;
    }
    .titulo-numero{
        text-align: center;
    }
}
</style>