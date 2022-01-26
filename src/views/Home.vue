<template>
  <div>
    <div class="hero-image">
   <Navbar/>
   <Hero/>
    </div>
    <Empleo/>
    <Talento/>
    <Servicios/>
    <div class="seccion-contacto">
    <Contacto/>
    </div>
  </div>
</template>

<script>
import Navbar from '@/components/SectionsComponents/Navbar.vue'
import Hero from '@/components/Hero.vue'
import Empleo from '@/components/Empleo.vue'
import Talento from '@/components/Talento.vue'
import Servicios from '@/components/Servicios.vue'
import Contacto from '@/components/Contacto.vue'
export default {
  name: 'Home',
  components: {
    Navbar,Hero,Empleo,Talento,Servicios,Contacto
  }
}
</script>
<style>
.hero-image {
  background-image: url("../assets/Hero.png");
  background-size: cover;
  background-position: center;
  height: 100vh;
  background-repeat: no-repeat;
}
.seccion-contacto{
  height: 45rem;
  background-image: url('../assets/ola.png');
  background-position: center;
  background-size: cover;
}
@media screen and (max-width:1024px){
    .seccion-contacto{
        height: auto;
    }
}
/* Pantallas extrageande */

@media screen and (min-width:1800px){
  .seccion-contacto{
    height: 57rem;
  }
}
</style>