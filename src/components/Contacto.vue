<template>
<section class="contacto" id="contacto">
    <div class="container">
        <div class="row">
            <div class="col-xl-6">
              <Sections titulo="Contacto" contenido="¿Necesitas más información? No te preocupes escribenos en cualquiera de nuestras redes"/>
                <div class="contacto-logos">
                    <img src="../assets/telefono.svg" alt="numeroConctacto">
                    <span>{{numeroContacto}}</span>
                </div>
                    <div class="contacto-logos">
                    <img src="../assets/mail.svg" alt="emailsvg">
                    <span>{{email}}</span>
                    </div>
            </div>
            <div class="col-xl-6">
                <form action="https://formsubmit.co/felipe_v_spd.com" method="POST" class="formulario">
                    <input type="text" name="name" required placeholder="Nombre y apellidos">
                    <textarea name="message" required cols="30" rows="10" placeholder="Escribe un mensaje"></textarea>
                    <input name="email" type="email" placeholder="Correo electrónico">
                    <button class="boton-form" type="submit">Enviar</button>
                </form>
            </div>
        </div>
    </div>
</section>
</template>

<script>
import Sections from '@/components/SectionsComponents/Sections.vue'
export default {
    name: 'Contacto',
    data() {
        return {
            numeroContacto: '+58 654 789 321',
            email:'emailcontacto@gmail.com'
        }
    },
    components:{
        Sections
    },
    }

</script>

<style>
.contacto{
    padding-top:19rem;
}
.formulario input{
    padding:0.8rem;
    width:70%;
    margin-top: 1rem;
    outline: none;
    border: none;
    border-radius: 0.8rem;
}
.contacto-logos{
    margin-top: 1rem;
}
.contacto-logos img{
    width: 2.3rem;
}
.contacto-logos span{
    padding-left: 1rem;
    color: #ffff;
}
.formulario textarea{
    height: 9rem;
    margin-top: 1rem;
    width: 70%;
    outline: none;
    border: none;
    padding: 0.8rem;
    border-radius: 0.8rem;
}
.formulario button{
    border: none;
    background-color: #23272F;
    display: block;
    width: 70%;
    margin-top: 1rem;
    padding: 0.8rem;
    color: #ffff;
    border-radius: 0.8rem;
}
/* Inicio MediaQueries */
@media screen and (max-width:1024px){
    .formulario{
        text-align: center;
    }
    .boton-form{
        margin:auto;
        margin-top: 2rem;
        margin-bottom: 2rem;
    }
    .contacto-logos{
        text-align: center;
    }
}

/* Final MediaQueries */
</style>