<template>
  <div>
      <div class="container">
 <b-navbar toggleable="lg" type="dark">
    <b-navbar-brand href="#"><img src="../assets/logoTrack.svg" alt=""></b-navbar-brand>
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" class="justify-content-end" is-nav>
      <b-navbar-nav>
        <b-nav-item href="#">{{Busquedaempleo}}</b-nav-item>
        <b-nav-item href="#">{{Busquedatalento}}</b-nav-item>
        <b-nav-item href="#">{{Servicios}}</b-nav-item>
        <b-nav-item href="#">{{Contacto}}</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
      </div>
 
</div>
</template>

<script>
export default {
    name:'Navbar',
    data(){
        return{
            Busquedaempleo:'Búsqueda de empleo',
            Busquedatalento:'Búsqueda de talento',
            Servicios:'Servicios',
            Contacto:'Contacto'
}
    },
}
</script>

<style>

</style>