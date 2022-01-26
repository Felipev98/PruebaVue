<template>
<section>
    <div class="titulo">
    <h2>{{titulo}}</h2>
    <p>{{contenido}}</p>
    </div>
</section>
</template>

<script>
export default {
    name: 'Sections',
        props:{
        titulo:{
            type:String,
        },
        contenido:{
            type:String,
        },
    },
}
</script>

<style>
.titulo h2{
      font-family: 'GardeGothic-Bold';

}
.titulo{
    color: #BFBFBF;
}
/* Inicio MediaQueries */
@media screen and (max-width:700px){
    .titulo{
        text-align: center;
    }
}

/* Final MediaQueries */
</style>