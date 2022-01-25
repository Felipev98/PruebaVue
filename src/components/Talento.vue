<template>
  <section class="talento">
      <div class="container">
          <div class="row">
              <div class="col-xl-6 col-empleo" >
                  <Sections titulo="Búsqueda de talento" contenido="is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. "/>
              </div>
              <div class="col-xl-6">
                  <div class="row">
                      <div class="col-xl-6">
                        <Pasos numero=1 titulopasos="Primer Paso" contenidopasos="lorepdkpdkepdkepkdep"/>
                      </div>
                      <div class="col-xl-6">
                        <Pasos numero=2 titulopasos="Segundo Paso" contenidopasos="lorepdkpdkepdkepkdep"/>
                      </div>
                  </div>
                  <div class="row">
                       <div class="col-xl-6">
                        <Pasos numero=3 titulopasos="Tercer Paso" contenidopasos="lorepdkpdkepdkepkdep"/>
                      </div>
                      <div class="col-xl-6">
                        <Pasos numero=4 titulopasos="Cuarto Paso" contenidopasos="lorepdkpdkepdkepkdep"/>
                      </div>
                  </div>
              </div>
          </div>
      </div>
  </section>
</template>
<script>
import Sections from '@/components/Sections.vue'
import Pasos from '@/components/Pasos.vue'
export default {
    name:'Talento',
    components:{
        Sections,Pasos
    },

}
</script>

<style>
.talento{
    height: auto;
}
</style>