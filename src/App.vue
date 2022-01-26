<template>
  <div id="app">
     <div class="boton-arriba-contenedor">
    <a href="#">
      <div class="volver-arriba">
        <i class="fas fa-chevron-up"></i>
      </div>
    </a>
  </div>
    <router-view/>
  </div>
</template>
<script>
export default {
  created () {
    window.addEventListener('scroll', this.handleScroll);
  },
  destroyed () {
    window.removeEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleScroll (event) {
   if(this.isUserScrolling = (window.scrollY > 100)){
    document.querySelector('.boton-arriba-contenedor').classList.add('show-')
   }else{
    document.querySelector('.boton-arriba-contenedor').classList.remove('show-')
   }
    }
    }
}
</script>
<style>
@font-face {
  font-family: 'GardeGothic-Bold';
  src: url(./assets/fonts/itc-avant-garde-gothic-bold.otf);
}
@font-face {
  font-family: 'GardeGothic-Book';
  src: url(./assets/fonts/BookRegular.otf);
}
#app{
  background: #23272F ;
  font-family: 'GardeGothic-Book';

}
.seccion{
  height: auto;
      padding-top: 4rem;

}
.boton-arriba-contenedor{
    position: fixed;
    bottom: 4rem;
    right: 4rem;
    width: 6.6rem;
    height: 6.6rem;
    z-index: -1;
}
.volver-arriba{
    width: 0rem;
    height: 0rem;
    background-color: #82DEBE;
    border-radius: 50%;
    cursor: pointer;
    top: 50%;
    transition: .2s;
    transform: translate(-50%,50%);
    transition: all 0.3s ease;
    box-shadow: 0px 7px 30px black;
}
.volver-arriba i{
    position: absolute;
    font-size: 1rem;
    top: 48%;
    left: 50%;
    transform: translate(-50%,50%) scale(0);
    color: white;
    transition: .2s;
}
.show-{
    z-index: 10;
    transform: translateX(125px);
}
.show- .volver-arriba{
    animation: popop .3s ease-in-out;
    width: 4rem;
    height: 4rem;
    z-index: 11;
}
.show- i{
    transform: translate(-50%,-50%) scale(1);
}

@keyframes popop {
    0%{
        width: 0rem;
        height: 0rem;
    }
    50%{
        width: 2rem;
        height: 2em;
    }
    100%{
        width: 4rem;
        height: 4rem;
    }
}
</style>
