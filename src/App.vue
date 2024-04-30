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
        <div class="botonMenu">
          <label for="labelMenu" class="menuLabel1">
            <img src="./assets/menu.png" class="menuIcono" alt="">
          </label>
        </div>
        <input type="checkbox" name="menu" id="labelMenu">
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
      <section class="app-main--estructure">
        <div class="app-container--main">
          <div class="app-boxes-one">    
                <div class="videoContainer">
                  <div class="videoContainerDivFloat">
                    <p class="videoContainerTextoOne">Escuela Karasuno</p>
                    <p class="videoContainerTextoTwo">"Surca los cielos"</p>
                  </div>
                <video autoplay loop muted class="video-seccion">
                  <source src="./assets/seccion.mp4" type="video/mp4">
                </video>
              </div> 
          </div>
          <div class="app-boxes-two">
            <h2 class="main-h2-down">Reglas</h2>
            <div class="textDown-3">
                <img class="subText-3" src="./assets/reglas.jpg" alt="">
                <p class="textDownParr-3">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dicta ex aliquam temporibus dolore quam consequuntur
                  itaque porro sapiente minus voluptate illum quaerat architecto voluptatem assumenda quisquam nesciunt, facilis cum consequatur!<br><br>
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tenetur minima voluptatum nisi earum sapiente
                  deserunt. Repellendus repudiandae nostrum, non quas facere perferendis rerum eos adipisci harum minus porro natus vitae?
                </p>
            </div>
          </div>
          <div class="app-boxes-three">  
            <div class="div4-seccion2">
              <h3 class="redes-sociales">Instagram</h3>
              <iframe class="instaGram" src="https://www.instagram.com/haikyuuu.official/embed/">
              </iframe>
            </div>      
          </div>
          <div class="app-boxes-four">
            <div class="textDown-1">
              <h2 class="main-h2-top">Quienes Somos</h2>
              <p class="textDownParr">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tenetur minima voluptatum nisi earum sapiente
                deserunt. Repellendus repudiandae nostrum, non quas facere perferendis rerum eos adipisci harum minus porro natus vitae?</p>
              <p class="textDownParr3">Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit similique nam tempora id quia esse officia porro nobis eaque
                Asperiores similique molestias culpa a quisquam vel voluptatibus repellat doloremque numquam.
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tenetur minima voluptatum nisi earum sapiente
                deserunt. Repellendus repudiandae nostrum, non quas facere perferendis rerum eos adipisci harum minus porro natus vitae?
                Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tenetur minima voluptatum nisi earum sapiente
                deserunt. Repellendus repudiandae nostrum, non quas facere perferendis rerum eos adipisci harum minus porro natus nalte?
              </p>
            </div>
          </div>
          <div class="app-boxes-five">
            <div class="div-faceb">
              <h3 class="redes-sociales">Facebook</h3>
              <apiFacebookReal/>             
            </div>
          </div>
          <div class="app-boxes-six">          
              <div class="textDown-2">
                <h2 class="main-h2-down">Reglas</h2>
              <div class="subText-2">
                <p class="textDownParr-2">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dicta ex aliquam temporibus dolore quam consequuntur
                  itaque porro sapiente minus voluptate illum quaerat architecto voluptatem assumenda quisquam nesciunt, facilis cum consequatur!<br><br>
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tenetur minima voluptatum nisi earum sapiente
                  deserunt. Repellendus repudiandae nostrum, non quas facere perferendis rerum eos adipisci harum minus porro natus vitae?
                </p>
              </div>
            </div>
          </div>
          <div class="app-sliderbox">
            <sliderFotos/>
          </div>
          <div class="app-slider--old">
            <!-- Video -->
            <section class="seccion1">
              <carruselDeVideos/>
            </section>
          </div>
        </div>
      </section>
      <!-- Galeria -->  
      <section class="seccion3">
          <div class="div-seccion3">
            <galleryNoCarru/>
          </div>
        </section>
    </div>
    <botonRedes/>
  </div> 
  </div>   
  <div v-show="isVisibleShow2" class="teamFull"><homeIniStartTwo/></div>
  <div v-show="isVisibleShow3" class="partidosAll"><homeIniStartThree/></div>
  <div v-show="isVisibleShow4" class="infoProject"><homeIniStartFour/></div>
  <div v-show="isVisibleShow5" class="contactWe"><homeIniStartFive/></div>
  <footerBeatiful/>
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
import footerBeatiful from './components/footerBeatiful.vue';
import sliderFotos from "./components/sliderFotos.vue";

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
  sliderFotos,
  botonRedes,
  footerBeatiful,
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
.app-main--estructure{
  display: flex;
  justify-content: center;
  background-color: rgb(255, 123, 0);
}
.app-container--main{
  display: grid;
  grid-template-columns: repeat(3, 1f);
  grid-template-rows: auto 1fr 0.9fr auto;
  background-color: rgb(39, 40, 40);
  width: 100%;
}
.app-boxes-one{
  display: flex;
  justify-content: center;
  flex-direction: column;
  grid-column: 1/4;
  grid-row: 1;
  width: 100%;
  margin:1em 0;
}
/* reglas con foto */
.app-boxes-two{
  grid-column: 1;
  grid-row: 4;
  height: 100%;
  background-color: rgb(53, 54, 68); 
}
/* Instagram */
.app-boxes-three{
  display: flex;
  justify-content: center;
  width: 100%;  
  height: 100%;
  grid-column: 1;
  grid-row: 2;
  background-color: rgb(53, 54, 68); 
  box-shadow: 0px -5px 5px rgba(0, 0, 0, 0.5);
}
.div4-seccion2 {
  height: 100%;
  font-family: 'DIMISTRI';
}
.instaGram{
  display: flex;
  justify-content: flex-end;
  height: 93%; 
  width: 23em;  
  border: 0.3em;
  box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.5);
}
/* cuadro en la mitad de las redes */
.app-boxes-four{
  grid-column: 2;
  grid-row: 2;
  box-shadow: 0px -5px 5px rgba(0, 0, 0, 0.5);
  width: 33vw;
}
/* facebook */
.app-boxes-five{
  display: flex;
  justify-content: center;
  align-items: center;
  grid-column: 3;
  grid-row: 2;
  background-color: rgb(53, 54, 68); 
  box-shadow: 0px -5px 5px rgba(0, 0, 0, 0.5);
}
.app-sliderbox{
  height: 100%;
  grid-column: 1/5;
  grid-row: 3;
  display: flex;
  justify-content: center;
  background-color: rgb(53, 54, 68);
  overflow: hidden;
}
.app-slider--old{
  display: flex;
  justify-content: center;
  align-content: flex-end;
  grid-column: 2;
  grid-row: 4;
  height: 100%;
  width: 100%;
}
.app-boxes-six{
  grid-column: 3;
  grid-row: 4;
  background-color: rgb(53, 54, 68); 
}
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
.menuIcono {
  height: 1px;
}
#labelMenu {
  display: none;
}
/* Mediaquery del header */
@media only screen and (min-width: 100px) and (max-width: 1025px) {
  .header {
    position: relative;
  }
  .divHeader {
    height: 40px;
    justify-content: flex-end;
  }
  .botonMenu {
    position: absolute;
    left: 0;
    right: auto;
    top: auto;
    bottom: 0;
    background-color: rgb(255, 123, 0);
    height: 2em;
    width: 100%;
    line-height: 40px;
    z-index: 100;
  }
  .menuIcono {
    height: 1.7em;
    /* margin-right: 10px; */
    display: initial;
    z-index: 130;
  }
  #labelMenu{
    display: none;
  }
  .ul-header {
    position: absolute;
    background: #234;
    width: 100%;
    height: auto;
    top: auto;
    left: 0;
    display: block;
    transition: all 500ms ease;
    transform: translateX(-100%);
    z-index: 1000;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 1em 0;
  }
  #labelMenu:checked ~ .ul-header {
    transform: translateX(0%);
  }
  .ul-header a {
    display: block;
    /* margin-top: 10px; */
  }
}
/* Video */
.seccion1 {
  width: 100%;
  height: 100%;
}
.videoContainer{
  display: flex;
  justify-content: center;
  align-items: center;
  /* background-color: rgba(255, 123, 0, 0.853); */
  width: 100%;
  position: relative;
}
.videoContainerDivFloat {
  position: absolute;
  top: auto;
  bottom: auto;
  left: auto;
  right: auto;
  width: 55%;
  z-index: 2;
  /* background-color: chartreuse; */
}
.videoContainerTextoOne {
  text-align: center;
  width: 100%;
  font-size: 70px;
  color: white; 
  text-shadow: -2px -2px 0 #000,  
                2px -2px 0 #000,
                -2px 2px 0 #000,
                2px 2px 0 #000; /* Contorno negro */
  padding: 0 1em;
  /* background-color: aqua; */
  border-bottom: 2px solid black;
}
.videoContainerTextoTwo {
  text-align: center;
  width: 100%;
  font-size: 40px;
  color: white; 
  text-shadow: -2px -2px 0 #000,  
                2px -2px 0 #000,
                -2px 2px 0 #000,
                2px 2px 0 #000; /* Contorno negro */
                /* background-color: blue; */
}
.video-seccion {
  width: 83%;
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
  text-align: center;
  color: rgb(255, 123, 0);
  margin-top: 0.5em;
  font-family: 'DIMISTRI', sans-serif;
}
.main-h2-top:hover{
  color: rgb(255, 255, 255);
}
.main-h2-down{
  display: flex;
  justify-content: center;
  text-align: center;
  background-color: rgb(53, 54, 68); 
  color: rgb(255, 123, 0);
  font-family: 'DIMISTRI', sans-serif;
}
.main-h2-down:hover{
  color: rgb(255, 255, 255);
}
.textDown-1{
  display: flex;
  justify-content: center;
  background-color: rgb(53, 54, 68); 
  flex-direction: column;
  height: 100%;
  margin: 0;
}
.textDown-1 p {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: justify;
  width: 90%;
  margin: 1em auto;
}
.textDown-2{
  display: flex;
  background-color: rgb(53, 54, 68); 
  flex-direction: column;
}
.textDown-3{
  display: flex;
  align-items: center;
  background-color: rgb(53, 54, 68);
  gap: 1em;
  height: auto;
}
.textDownParr{
  margin: 0;
  color: rgb(255, 255, 255);
}
.textDownParr3{
  display: flex;
  flex-direction: column;
  color: rgb(255, 255, 255);
  margin: 0;
  padding-bottom: 2em;
}
.subText-2 {
  display: flex;
  height: 50%;
  width: 90%;
}
.subText-3{
  height: 20em;
  width: 10em;
  padding-bottom: 80px;
  margin-top: 5em;
  margin-left: 0.5em;
}
.textDownParr-3{
  color: rgb(253, 253, 253);
  display: flex;
  flex-direction: column;
  text-align: justify;
  width: 50%;
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
  text-align: justify;
}
.redes-sociales {
  display: flex;
  justify-content: center;
  font-size: 30px;
  color: rgb(255, 123, 0);
  margin-top: 0.5em;
  margin-bottom: 0.5em;
}
.redes-sociales:hover{
  color: rgb(255, 255, 255);
}
.div-faceb {
  padding: 0;
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
/* Footer */
.footer{
  height: 2em;
  background-color: black;
  display: flex;
  justify-content: center;
  align-items: center;
  color: azure;
}
.footer:hover{
  color: rgba(255, 10, 6, 0.883);
}
/* Medidaquery del responsive */
@media only screen and (min-width: 100px) and (max-width: 1025px) {
/* Texto del video abajo de los botones */
  .videoContainerTextoOne {
  text-align: center;
  width: 100%;
  font-size: 2.28em;
  color: white; 
  text-shadow: -2px -2px 0 #000,  
                2px -2px 0 #000,
                -2px 2px 0 #000,
                2px 2px 0 #000; /* Contorno negro */
  padding: 0 1em;
  /* background-color: aqua; */
  border-bottom: 2px solid black;
}
.videoContainerTextoTwo {
  text-align: center;
  width: 100%;
  font-size: 1.4em;
  color: white; 
  text-shadow: -2px -2px 0 #000,  
                2px -2px 0 #000,
                -2px 2px 0 #000,
                2px 2px 0 #000; /* Contorno negro */
                /* background-color: blue; */
}
  /* Cuerpo con Grid */
.seccion2 {
  display: flex;
  flex-direction: column;
}
.textDown-1{
  display: flex;
  justify-content: center;
  background-color: rgb(53, 54, 68); 
  flex-direction: column;
}
.textDown-1 p {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: justify;
  width: 80%;
}
.textDown-2{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;  
  background-color: rgb(53, 54, 68); 
  height: 100%;
  box-shadow: 0px -3px 3px rgba(0, 0, 0, 0.5), 0px 3px 3px rgba(0, 0, 0, 0.5);
  z-index: 5;
}
.subText-2{
  /* display: flex; */
  height: 100%;
}
.subText-2 p {
  padding-left: 0;
}
.textDownParr{
  display: flex;
  flex-direction: column;
  color: rgb(255, 255, 255);
  margin: 0;
}
.textDownParr3{
  display: flex;
  flex-direction: column;
  color: rgb(255, 255, 255);
  margin: 0;
  padding-bottom: 2em;
}
.app-boxes-two{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  grid-column: 1;
  grid-row: 6;
  box-shadow: 0px -3px 3px rgba(0, 0, 0, 0.5), 0px 3px 3px rgba(0, 0, 0, 0.5);
  padding-bottom: 1.6em;
  z-index: 5;
}
.textDown-3{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  background-color: rgb(53, 54, 68); 
  margin-top: 1em;
}
.subText-3{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 0;
  margin: 0;
  height: 45%;
  width: 35%;
}
.textDownParr-2{
  color: rgb(253, 253, 253);
  display: flex;
  flex-direction: column;
  padding-bottom: 1em;
}
.textDownParr-3{
  color: rgb(253, 253, 253);
  display: flex;
  flex-direction: column;
  text-align: justify;
  width: 72%;
}
.redes-sociales {
  display: flex;
  justify-content: center;
  font-size: 30px;
  color: rgb(255, 123, 0);
}
.div-faceb {
  padding: 0;
  margin: 0;
  height: 100%; 
  font-family: 'DIMISTRI';
  padding-bottom: 2em;
}
.app-container--main{
  display: grid;
  grid-template-columns: 1f;
  grid-template-rows: auto auto 1fr 20em auto;
  background-color: rgb(39, 40, 40);
  width: 100%;
}
.app-boxes-one{
  display: flex;
  justify-content: center;
  flex-direction: column;
  grid-column: 1;
  grid-row: 1;
  width: 100%;
  margin:1em 0;
}
/* cuadro en la mitad de las redes */
.app-boxes-four{
  display: flex;
  justify-content: center;
  grid-column: 1;
  grid-row: 2;
  box-shadow: 0px -5px 5px rgba(0, 0, 0, 0.5);
  width: 100%;
}
/* facebook */
.app-boxes-five{
  display: flex;
  justify-content: center;
  align-items: center;
  grid-column: 1;
  grid-row: 3;
  background-color: rgb(53, 54, 68); 
  box-shadow: 0px -1px 1px rgba(0, 0, 0, 0.5);
}
.app-slider--old{
  display: flex;
  justify-content: center;
  align-content: flex-end;
  grid-column: 1;
  grid-row: 4;
  height: 100%;
  width: 100%;
  margin: 0.2em 0;
}
.seccion1 {
  width: 100%;
  height: 100%;
}
/* Instagram */
.app-boxes-three{
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
  width: 100%;  
  grid-column: 1;
  grid-row: 5;
  background-color: rgb(53, 54, 68); 
  /* box-shadow: 0px -1px 1px rgba(0, 0, 0, 0.5); */
  margin-top: 0.4em;
  padding-bottom: 1.5em;
}
.div4-seccion2 {
  height: 30rem;
  padding-bottom: 3em;
  font-family: 'DIMISTRI';
}
.instaGram{
  display: flex;
  height: 90%;  
  width: 100%;
}
/* reglas con foto */
.app-sliderbox{
  height: 100%;
  grid-column: 1;
  grid-row: 7;
  display: flex;
  justify-content: center;
  background-color: rgb(53, 54, 68);
  overflow: hidden;
}
.app-boxes-six{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  grid-column: 1;
  grid-row: 8;
  height: 100%;
}
.main-h2-down{
  display: flex;
  justify-content: center;
  text-align: center;
  flex-direction: column;
  color: rgb(0, 0, 0);
  background-color: rgb(53, 54, 68); 
  font-family: 'DIMISTRI', sans-serif;
  margin-top: 1em;
}
.main-h2-down:hover{
  color: rgb(255, 123, 0);
}
}
</style>