<!-- pendiente
Colocar el carrucel automatico que vaya pasando de cosas y al inicio
Arreglar el titulo de las redes sociales y que no parezcan anuncios
cambiar la letra
y colocar abajo videos aleatorios para que la gente se entretenga
y colocar en el texto de reglas algo gris para evitar que sea tanto naranjado
y los links de los videos hipervinculados para que los lleve al youtube de cada video.
numeros de contacto información demografica lugar de entrenamiento hora un mapa de google map y
las rutas, que servicios prestamos, en equipo mision vision quienes somos, en partidos colocar el calendario
y cronograma, noticias
en quienes somos los acontecimientos importantes, actualidad
en la pagina de información poner la descripcion de cada jugador osea todos que así sean 30 
más adelante colocar un grupo de fans con usuario registrado para hacer comunidad.
-->
<template>
  <div>
    <!-- Header -->
    <header class="header"> 
      <div class="div-header">
        <ul class="ul-header">
          <li class="btn-header sepBtn border-li1"><a @click="clickEvent('homeIni')" class="aBtn" href="#">Inicio</a></li>
          <li class="btn-header sepBtn"><a @click="clickEvent('teamFull')" class="aBtn" href="#">Equipo</a></li>
          <li class="btn-header sepBtn"><a @click="clickEvent('partidosAll')" class="aBtn" href="#">Partidos</a></li>
          <li class="btn-header sepBtn border-li2"><a @click="clickEvent('infoProject')" class="aBtn" href="#">Informacion</a></li>
          <li class="btn-header sepBtn"><a @click="clickEvent('contactWe')" class="aBtn" href="#">Contactanos</a></li>
        </ul>
      </div>
    </header> 
    <div class="bodyHide" v-show="bodyHideBd">
      <div class="homeIni" v-show="appView">
      <!-- Cuerpo -->
      <section class="seccion2">
        <div class="div1-seccion2">
          <div class="div1SeccionTwo">
            <p class="divInvi"></p>
          </div>
        <div class="textDown-1">
          <h2 class="main-h2-top">Quienes Somos</h2>
        <p class="textDownParr">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tenetur minima voluptatum nisi earum sapiente
          deserunt. Repellendus repudiandae nostrum, non quas facere perferendis rerum eos adipisci harum minus porro natus vitae?</p>
        <p class="textDownParr">Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit similique nam tempora id quia esse officia porro nobis eaque
          Asperiores similique molestias culpa a quisquam vel voluptatibus repellat doloremque numquam.
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tenetur minima voluptatum nisi earum sapiente
          deserunt. Repellendus repudiandae nostrum, non quas facere perferendis rerum eos adipisci harum minus porro natus vitae?
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tenetur minima voluptatum nisi earum sapiente
          deserunt. Repellendus repudiandae nostrum, non quas facere perferendis rerum eos adipisci harum minus porro natus vitae?
        </p>
        </div>
        </div>
        <div class="div2-seccion2">
          <div class="div1SeccionTwo">
            <p class="divInvi2"></p>
          </div>
          <div class="textDown-2">
          <h2 class="main-h2-down">Reglas</h2>
          <div class="subText-2">
            <img src="./assets/reglas.jpg" alt="">
            <p class="textDownParr-2">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dicta ex aliquam temporibus dolore quam consequuntur
              itaque porro sapiente minus voluptate illum quaerat architecto voluptatem assumenda quisquam nesciunt, facilis cum consequatur!<br><br>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tenetur minima voluptatum nisi earum sapiente
              deserunt. Repellendus repudiandae nostrum, non quas facere perferendis rerum eos adipisci harum minus porro natus vitae?</p>
          </div>
          </div>
          </div>
          <div class="div3-seccion2">
            <div class="div-faceb">
              <h3 class="redes-sociales">Facebook</h3>
              <apiFacebookReal/>             
            </div>
          </div>
          <div class="div4-seccion2">
              <h3 class="redes-sociales">Instagram</h3>
            <iframe class="instaGram" src="https://www.instagram.com/haikyuuu.official/embed/">
            </iframe>
          </div>
        </section>
                      <!-- Video -->
    <section class="seccion1">
      <carruselDeVideos/>
    </section>
      <!-- Galeria -->  
      <section class="seccion3">
          <div class="div-seccion3">
            <galleryNoCarru/>
            <div>            
              <div class="videoContainer">
              <video autoplay loop muted class="video-seccion">
                <source src="./assets/seccion.mp4" type="video/mp4">
              </video>
              </div>
            </div>
          </div>
        </section>
        <section class="seccion4">
          <p class="footerText"> pLorem ipsum dolor sit amet.
          pLorem ipsum1 dolor sit amet consectetur adipisicing elit. Necessitatibus perferendis ullam fugit sint natus quis quaerat! Dolorum, debitis. Soluta totam molestias, dolorem neque unde esse nisi quod facilis laudantium quibusdam!
          pLorem ipsum dolor sit amet consectetur adipisicing elit. Necessitatibus perferendis ullam fugit sint natus quis quaerat! Dolorum, debitis. Soluta totam molestias, dolorem neque unde esse nisi quod facilis laudantium quibusdam!4</p>
        <div class="socialMedia">
        <img class="footerLogo" src="./assets/logo.png" alt="">
        </div>
        </section>
    </div>
    <botonRedes/>
    </div> 
  </div>   
  <!-- <div v-show="isVisibleShow" class="homeIni1"><homeIniStart/></div> No tocar -->
  <div v-show="isVisibleShow2" class="teamFull"><homeIniStartTwo/></div>
  <div v-show="isVisibleShow3" class="partidosAll"><homeIniStartThree/></div>
  <div v-show="isVisibleShow4" class="infoProject"><homeIniStartFour/></div>
  <div v-show="isVisibleShow5" class="contactWe"><homeIniStartFive/></div>
  <footer class="footer">
    &copy; Moncada, Ballestero & Jill Angel LLC, a subsidiary of Compas del codigo de hierro, 2024 Inc. All Rights Reserved.
  </footer>
</template>

<script>
import galleryNoCarru from "./components/galleryNoCarru.vue";
import apiFacebookReal from "./components/apiFacebookReal.vue";
// import homeIniStart from "./components/homeIniStart.vue" No tocar;
import homeIniStartTwo from "./components/homeIniStartTwo.vue";
import homeIniStartThree from "./components/homeIniStartThree.vue";
import homeIniStartFour from "./components/homeIniStartFour.vue";
import homeIniStartFive from "./components/homeIniStartFive.vue";
import carruselDeVideos from "./components/carruselDeVideos.vue";
import botonRedes from './components/botonRedes.vue';
export default {
  components: {
  galleryNoCarru,
  apiFacebookReal,
  // homeIniStart No tocar,
  homeIniStartTwo,
  homeIniStartThree,
  homeIniStartFour,
  homeIniStartFive,
  carruselDeVideos, 
  botonRedes,
},
  data() 
  {
    return {
    bodyHideBd: true,
    appView: true,
    isVisibleShow: false,
    isVisibleShow2: false,
    isVisibleShow3: false,
    isVisibleShow4: false,
    isVisibleShow5: false,
    };
  },
  methods: {
    clickEvent(componentName) {
      this.appView = false;
      this.isVisibleShow = false;
      this.isVisibleShow2 = false;
      this.isVisibleShow3 = false;
      this.isVisibleShow4 = false;
      this.isVisibleShow5 = false;     
      switch (componentName) {
        case 'homeIni':
          this.appView = true;
          break;
        case 'teamFull':
          this.isVisibleShow2 = true;
          break;
        case 'partidosAll':
          this.isVisibleShow3 = true;
          break;
        case 'infoProject':
          this.isVisibleShow4 = true;
          break;
        case 'contactWe':
          this.isVisibleShow5 = true;
          break;
        default:
          break;
      }
    }
  },
}
  </script>

<style>
@font-face {
  font-family: 'DIMIS___';
  src: url('./assets/fonts/DIMIS___.TTF') format('truetype');
}
@font-face {
  font-family: 'DIMISTRI';
  src: url('./assets/fonts/DIMISTRI.TTF') format('truetype');
}
/* Global */
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
/* Header */
.header {
  width: 100%;
  height: 32vh;
  display: flex;
  background-image: url("./assets/header.png");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center center;
  margin: 0;
  padding: 0; 
  box-sizing: border-box;
  justify-content: center;
  align-items: end;
}
.ul-header {
  list-style: none;
  display: flex;
  margin: 0;
  padding: 0;
}
.aBtn{
  display: flex;
  justify-content: center;
  font-family: 'DIMIS___', sans-serif;
}
/* Botones */
.btn-header a {
  display: flex;
  text-decoration: none;
  background-color: rgb(255, 123, 0);
  color: rgb(250, 245, 245);
  padding: 10px;
  font-size: 20px;
  transition: 1s;
  transform: skewX(-15deg);
  border: none;
  box-shadow: 6px 6px 0 black;
  border-right: 1px solid black;
  animation: color_anim 1s infinite 0.2s;
  margin: 0.3em;
  z-index: 9999;
  letter-spacing: 0.5px;
}
.border-li1 a {
  display: flex;
  justify-content: center;
  transition: 1s;
  box-shadow: 6px 6px 0 black;
  transform: skewX(-15deg);
  animation: color_anim 1s infinite 0.2s;

}
.border-li2 a {
  display: flex;
  justify-content: center;
  transition: 1s;
  box-shadow: 6px 6px 0 black;
  transform: skewX(-15deg);
  border-right: 1px solid black;
  animation: color_anim 1s infinite 0.2s;
}
.border-li1 a:hover {
  transition: 0.5s;
  box-shadow: 6px 6px 0 black;
  animation: color_anim 1s infinite 0.2s;
}
.border-li2 a:hover {
  transition: 0.5s;
  box-shadow: 6px 6px 0 black;
  animation: color_anim 1s infinite 0.2s;
}
.btn-header a:hover{
  background-color: rgba(255, 10, 6, 0.883);
  color: rgb(0, 0, 0);
  padding: 10px;
}
.sepBtn{
  /* Otra subclass del ul-header */
  padding-left: 5px;
  width: 10em;
}
/* Video */
.seccion1 {
  position: relative;
  width: 100%;
  height: 100%;
  overflow: hidden;
}
.videoContainer{
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: rgba(255, 123, 0, 0.853);
}
.video-seccion {
  width: 50em;
  height: auto;
} 
/* Cuerpo con Grid */
.seccion2 {
  display: grid;
  grid-template-columns: 8fr 2fr;
  grid-template-rows: 1fr 1fr;
}
.main-h2-top{
  display: flex;
  justify-content: center;
  padding: 1em;
  text-align: center;
  color: rgb(8, 8, 8);
  font-family: 'DIMISTRI', sans-serif;
}
.main-h2-top:hover{
  color: rgb(255, 123, 0);
}
.main-h2-down{
  display: flex;
  justify-content: center;
  padding: 25px;
  margin-left: 6em;
  text-align: center;
  color: rgb(0, 0, 0);
  font-family: 'DIMISTRI', sans-serif;
}
.main-h2-down:hover{
  color: rgb(255, 123, 0);
}
p{
  display: flex;
  justify-content: center;
  text-align: justify;
  color: rgb(0, 0, 0);
  width: 95%;
}
/* Cajas del Grid */
.div1-seccion2 {
  /* Izquierda arriba */
  grid-column: 1;
  grid-row: 1;
  background-color: rgb(255, 123, 0);
  padding: 10px;
  height: 26em;
  text-align: justify;
  padding-bottom: 5px;
}
.div1SeccionTwo{
  background-color: rgba(31, 33, 70, 0);
}
.div2-seccion2 {
    /* Izquierda abajo */
  grid-column: 1;
  grid-row: 2;
  background-color: rgb(255, 123, 0);
  padding: 15px 10px;
  height: 26em;
  padding-top: 5px;
}
.textDown-1{
  display: flex;
  justify-content: center;
  background-color: rgb(53, 54, 68); 
  flex-direction: column;
  height: 100%;
  border-radius: 15px;
}
.textDown-1 p {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: justify;
  width: 90%;
  margin: 15px auto;
}
.textDown-2{
  background-color: rgb(53, 54, 68); 
  flex-direction: column;  
  height: 100%;
  border-radius: 15px;
}
.textDownParr{
  color: rgb(255, 255, 255);
}
.subText-2 {
  display: flex;
  flex-direction: row;
  height: 50%;
  width: 90%;
}
.subText-2 img {
  height: 20em;
  width: 14em;
  padding-bottom: 80px;
  padding-left: 30px;
  padding-right: 20px;
}
.subText-2 p {
  padding-top: 10px;
  margin: 10px;
  padding-left: 30px;
}
.textDownParr-2{
  color: rgb(253, 253, 253);
  display: flex;
  flex-direction: column;
}
.div3-seccion2 {
  /* Facebook */
  background-color: #353644;
  grid-column: 2;
  grid-row: 1;
  display: flex;
  justify-content: center;
  padding: 5px;
  height: 26em;
  width: 100%;
  border-left: rgb(56, 56, 56, 0.3) 2px solid;
  font-family: 'DIMISTRI';
}
.redes-sociales {
  display: flex;
  justify-content: center;
  font-size: 30px;
  color: rgb(255, 123, 0);
}
.div-faceb {
  position: relative;
  padding: 0;
  height: 27em; 
  width: 100%;
  overflow: hidden;
}
.instaGram{
  width: 270px;  
  height: 93%; 
  border: 5px;
  box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.5);
}
.div4-seccion2 {
  /* Instagram */
  border-left: rgb(56, 56, 56, 0.3) 2px solid;
  grid-row: 2;
  grid-column: 2;
  background-color: blue;
  padding: 10px 0;
  background-color: #353644;
  height: 100%;
  font-family: 'DIMISTRI';
}
/* Gallery */
.div-seccion3{
  background-color: rgb(56, 56, 56); 
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  padding: 10px;
  height: 100%;
}
/* Antes del footer */
.seccion4 {
  height: 100%;
  width: 100%;
  background-color: rgb(255, 123, 0);
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: justify;
  color: white;
  padding: 15px;
}
.footerText{
  border-right: rgb(56, 56, 56, 0.5) 1px solid;
  padding: 10px;
}
.footerLogo {
  width: 180px;
  height: 200px;
}
/* Footer */
.footer{
  background-color: black;
  display: flex;
  justify-content: center;
  align-items: center;
  color: azure;
  padding-top: 15px;
  padding-bottom: 4px;
}
.footer:hover{
  color: rgba(255, 10, 6, 0.883);
}
</style>
