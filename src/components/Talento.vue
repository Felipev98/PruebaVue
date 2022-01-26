<template>
  <section class="seccion" id="talento">
      <div class="container">
          <div class="row">
              <div class="col-xl-6 col-empleo" >
                  <Sections titulo="Búsqueda de talento" contenido="Se nos dice constantemente que el mundo esta cambiando, que las grandes organizaciones exigen cada vez más profesionales competentes y alineados  a la avanzada tecnología. Y esto es cierto. En la búsqueda del crecimiento, posicionamiento y diferenciación, las empresas contratan a los mejores talentos. Es por ello que es muy importante disponer de herramientas que permitan agilizar estos procesos. Conoce el proceso de nuestra webapp: "/>
              </div>
              <div class="col-xl-6">
                  <div class="row">
                      <div class="col-xl-6">
                        <Pasos numero='1' titulopasos="Registro en la web" contenidopasos="Registrate en nuestra web para empezar tu proceso de búsqueda de talento"/>
                      </div>
                      <div class="col-xl-6">
                        <Pasos numero='2' titulopasos="Armar perfil" contenidopasos="Añade las características de tu empresa y sector"/>
                      </div>
                  </div>
                  <div class="row">
                       <div class="col-xl-6">
                        <Pasos numero='3' titulopasos="Cargar datos" contenidopasos="Muestra toda la información referente a tu empresa"/>
                      </div>
                      <div class="col-xl-6">
                        <Pasos numero='4' titulopasos="Subir oferta" contenidopasos="Publica tu oferta de trabajo"/>
                      </div>
                  </div>
              </div>
          </div>
      </div>
  </section>
</template>
<script>
import Sections from '@/components/SectionsComponents/Sections.vue'
import Pasos from '@/components/SectionsComponents/Pasos.vue'
export default {
    name:'Talento',
    components:{
        Sections,Pasos
    },

}
</script>

<style>
</style>