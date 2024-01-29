<template>
  <div>
    <header class="header"> 
    </header>
    <nav class="nav">
      <div class="div-header">
        <ul class="ul-nav">
          <li class="btn-header sepBtn border-li1"><a href="#">Inicio</a></li>
          <li class="btn-header sepBtn"><a class="aBtn" href="#">Contactanos</a></li>
          <li class="btn-header sepBtn"><a class="aBtn" href="#">Equipo</a></li>
          <li class="btn-header sepBtn"><a class="aBtn" href="#">Partidos</a></li>
          <li class="btn-header sepBtn border-li2"><a href="#">Informacion</a></li>
        </ul>
      </div>
      </nav>
      <section class="seccion1">
        <div class="videoContainer">
        <video autoplay loop muted class="video-seccion">
          <source src="./assets/seccion.mp4" type="video/mp4">
        </video>
        </div>
        </section>
      <section class="seccion2">
        <div class="div1-seccion2">
          <div class="div1SeccionTwo">
            <p class="divInvi"></p>
          </div>
          <h2>Quienes Somos</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tenetur minima voluptatum nisi earum sapiente
          deserunt. Repellendus repudiandae nostrum, non quas facere perferendis rerum eos adipisci harum minus porro natus vitae?</p>
        </div>
        <div class="div2-seccion2">
          <div class="div1SeccionTwo">
            <p class="divInvi2"></p>
          </div>
          <h2>Reglas</h2>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dicta ex aliquam temporibus dolore quam consequuntur
            itaque porro sapiente minus voluptate illum quaerat architecto voluptatem assumenda quisquam nesciunt, facilis cum consequatur!</p>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tenetur minima voluptatum nisi earum sapiente
          deserunt. Repellendus repudiandae nostrum, non quas facere perferendis rerum eos adipisci harum minus porro natus vitae?</p>
        
          </div>
          <div class="div3-seccion2">
            <apiFacebookReal/>      
          </div>
          <div class="div4-seccion2">
            <iframe class="instaGram" src="https://www.instagram.com/haikyuuu.official/embed/">
            </iframe>
          </div>
        </section>
        <section class="seccion3">
          <div class="div-seccion3">
          <h2 class="galer"> Galería
          </h2>
          <apiFacebook/>
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
        <footer class="footer">
          &copy; Wizards of the Coast LLC, a subsidiary of Hasbro, Inc. All Rights Reserved.
        </footer>
  </div>
</template>

<script>
import apiFacebook from "./components/apiFacebook.vue";
import apiFacebookReal from "./components/apiFacebookReal.vue";
export default {
  components: {
  apiFacebook,
  apiFacebookReal,
}
}
</script>

<style>
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
}
/* .div-logo {
  display: flex;
  justify-content: center;
  align-items: center;
}
.logo {
  width: 180px;
  height: 200px;
} */
/* Nav */
.nav {
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: rgb(255, 157, 0);
  width: 100%;
  height: 60px;
}
.ul-nav {
  list-style: none;
  display: flex;
  margin: 0;
  padding: 0;
}
.aBtn{
  display: flex;
  justify-content: center;
}
/* Botones */
.btn-header a {
  display: flex;
  text-decoration: none;
  background-color: rgb(255, 123, 0);
  color: rgb(255, 255, 255);
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
  color: rgb(255, 255, 255);
  padding: 10px;
}
.sepBtn{
  padding-left: 5px;
  width: 10em;
}
/* Video */
.seccion1 {
  position: relative;
  width: 100%;
  height: 23em;
  overflow: hidden;
}
.videoContainer{
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: rgb(255, 123, 0);
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
h2 {
  padding: 25px;
  text-align: center;
  color: aliceblue;
}
h2:hover{
  color:rgb(53, 54, 68);
}
.galer{
  padding: 10px;
  text-align: center;
  color: aliceblue;
}
.galer:hover{
  color: rgb(255, 166, 0)
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
  grid-row: 1;
  grid-column: 1;
  background-color: rgb(255, 166, 0);
  padding: 30px;
  height: 26em;
  text-align: justify;
}
.div1SeccionTwo{
  background-color: rgb(53, 54, 68, 0.0);
  border-bottom: 0.4vh solid rgb(0, 0, 0, 0.2);
}
.div2-seccion2 {
  grid-row: 2;
  grid-column: 1;
  background-color: rgb(255, 166, 0);
  padding: 30px;
  height: 26em; 
}
.div3-seccion2 {
  background-color: rgb(255, 166, 0);
  grid-row: 1;
  grid-column: 2;
  display: flex;
  justify-content: center;
  padding: 10px 0;
  height: 26em;
  border-left: rgb(56, 56, 56, 0.3) 2px solid;
}
.instaGram{
  width: 270px;  
  height: 400px; 
  margin-top: 25px;
}
.div4-seccion2 {
  grid-row: 2;
  grid-column: 2;
  background-color: blue;
  padding: 10px 0;
  background-color: rgb(255, 166, 0);
  height: 26em;
  border-left: rgb(56, 56, 56, 0.3) 2px solid;
}
/* Gallery */
.div-seccion3{
  background-color: rgb(56, 56, 56); 
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  padding: 10px;
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
  padding: 5px;
}
.footer:hover{
  color: rgb(110, 110, 110);
}
</style>
