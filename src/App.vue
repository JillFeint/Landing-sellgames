<template>
<div class="container">
  <div class="text-top">
    <h1 class="unic-tittle">Venta de juegos de Steam <br>
      <br>  
      <img class="steam-logo" src="./assets/steam-icon.png" alt="">
    </h1>
  </div>
  <div class="redes-style">
    <a target="_blank" href="https://m.me/aleramrami/"><img class="redes" src="./assets/mensaje.png" alt=""></a>     
    <a target="_blank" href="https://wa.me/573014983594"><img class="redes" src="./assets/wps.png" alt=""></a>   
    <a target="_blank" href="https://www.facebook.com/groups/elmundodejill"><img class="redes" src="./assets/facebook.png" alt=""> </a>   
  </div>
  <div class="info">
    <p class="text-info"> Si necesitas juegos, ítems o saldo steam a un bajo precio, aquí estoy yo para colaborarte, 
      solo necesitas enviarme un mensaje, contáctate conmigo en alguna 
      de las redes sociales que están en la parte superior, para que podamos negociar como va ser el proceso, anímate...</p>
  </div>
  <div class="gallery">
    <gallgames/>
  </div>
  <!-- 
  <div class="carrusel2">
    hola culito
  </div>
  <div class="carrusel3">
    hola culito
  </div>
  -->
</div> 
<footer class="down"><p class="parr-footer"> ⊂ (◉‿◉) つ Cllykoji Gameshop ❦ 2024 </p></footer>
</template>

<script>
import gallgames from "./components/gall-games.vue"
export default {
  components: {
    gallgames,
  }
}
</script>

<style>
body {
  display: flex;
  justify-content: center;
  align-content: center;
  background-color: rgb(23, 33, 69);
}
.container{
  display: grid;
  grid-template-columns: repeat(4, 1fr);;
  grid-template-rows: repeat(5, 1fr);;
  justify-items: center;
  align-items: center; 
  width: 100vh;
  height: 100vh;
}
.text-top{
  grid-column: 2/4;
  grid-row: 2;
  width:55vh;
  height:auto;
}
.unic-tittle{
  text-align: center;
  color: rgb(255, 254, 254);
  animation: fuego-azul 1s infinite alternate;
}
@keyframes fuego-azul {
  0% {
    color: #4287f5; /* Color inicial azul */
    text-shadow: 0 0 10px #4287f5, 0 0 20px #4287f5, 0 0 40px #4287f5, 0 0 80px #4287f5;
  }
  100% {
    color: #00ffff; /* Color final cyan */
    text-shadow: 0 0 5px #4287f5, 0 0 10px #4287f5, 0 0 20px #2c6ac6, 0 0 40px #0088ff; 
  }
}
.steam-logo{
  width: auto;
  height: 6em;
}
.steam-logo:hover{
  animation: animacionImagen 3s infinite alternate;
}
@keyframes animacionImagen {
  0% {
    transform: scale(1); 
  }
  100% {
    transform: scale(1.2); 
  }
}
.redes-style {
  display: flex;
  justify-content: end;
  grid-column: 6;
  grid-row: 1;
  width: 30vh;
  height: 10vh;
  padding-top: 5px;
}
.info{
  grid-column: 1/5;
  grid-row: 3;
  color:rgb(255, 255, 255);
  width: 100vh;
  height: auto;
  text-align: justify;
  padding-bottom: 20px;
}
.text-info{
  animation: text-change 3s infinite alternate; /* Animación de cambio de color durante 3 segundos, alternando infinitamente */
}
@keyframes text-change{
  0% {
    color: #c1b5b5; /* Blanco */
  }
  50% {
    color: #c6d6f4; 
  }
  100% {
    color: #ffffff;
  }
}
.redes {
  width: auto;
  height: 2em;
  padding: 5px;
}
.redes:hover{
  width: auto;
  height: 2.2em;
}
.down {
  background-color:  rgb(15, 26, 66); /* Color de fondo con opacidad */
  color: #ffffff;
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
  animation: slideUp 1.5s ease-in-out;
}

@keyframes slideUp {
  0% {
    transform: translateY(100%);
  }
  100% {
    transform: translateY(0);
  }
}
.parr-footer{
  font-size: 13px;
  text-align: center;
  margin: 0;
  padding: 5px;
}
.parr-footer:hover{
  color: #4287f5;
}
.gallery{
  grid-column: 1/4;
  grid-row: 5;
  width: 73vh;
  height: 80vh;
}
/* .carrusel1{
  grid-column: 1;
  grid-row: 4;
  background-color: rgb(65, 206, 81);
  width: 25vh;
  height: 25vh;
}
.carrusel2{
  grid-column: 2;
  grid-row: 4;
  background-color: rgb(248, 0, 223);
  width:  25vh;
  height: 25vh;
}
.carrusel3{
  grid-column: 3;
  grid-row: 4;
  background-color: rgb(255, 153, 0);
  width: 25vh;
  height: 25vh;
}
.carrusel4{
  grid-column: 4;
  grid-row: 4;
  background-color: rgb(255, 0, 0);
  width: 25vh;
  height: 25vh;
} */
</style>
