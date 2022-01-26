<template>
  <div>
  <div class="container">
 <b-navbar toggleable="lg" type="dark">
    <b-navbar-brand class="logo-navbar" href="#"><img src="../../assets/logoTrack.svg" alt=""></b-navbar-brand>
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
    <b-collapse id="nav-collapse" class="justify-content-end" is-nav>
      <b-navbar-nav>
        <b-nav-item href="#empleo">{{Busquedaempleo}}</b-nav-item>
        <b-nav-item href="#talento">{{Busquedatalento}}</b-nav-item>
        <b-nav-item href="#servicios">{{Servicios}}</b-nav-item>
        <b-nav-item href="#contacto">{{Contacto}}</b-nav-item>
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
.navbar-nav{
    font-family: 'GardeGothic-Bold';
}
/* Inicio MediaQueries */
@media screen and (max-width:700px){
.logo-navbar img {
  width:12rem;
}
}
@media screen and (max-width:991px){
  .navbar-nav{
    background-color: #82DEBE;
    padding: 1rem;
  }
  li.nav-item{
    padding: 1rem;
  }
}
/* Final MediaQueries */

</style>