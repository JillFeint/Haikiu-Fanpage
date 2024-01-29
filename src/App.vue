<template>
  <div>
    <header class="header"> 
    </header>
    <nav class="nav">
      <div class="div-header">
        <ul class="ul-nav">
          <li class="btn-header border-li1"><a href="#">Inicio</a></li>
          <li class="btn-header sepBtn"><a href="#">Contactanos</a></li>
          <li class="btn-header sepBtn"><a href="#">Equipo</a></li>
          <li class="btn-header sepBtn"><a href="#">Partidos</a></li>
          <li class="btn-header border-li2"><a href="#">Informacion</a></li>
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
          <p> pLorem ipsum dolor sit amet.
          pLorem ipsum1 dolor sit amet consectetur adipisicing elit. Necessitatibus perferendis ullam fugit sint natus quis quaerat! Dolorum, debitis. Soluta totam molestias, dolorem neque unde esse nisi quod facilis laudantium quibusdam!
          pLorem ipsum dolor sit amet consectetur adipisicing elit. Necessitatibus perferendis ullam fugit sint natus quis quaerat! Dolorum, debitis. Soluta totam molestias, dolorem neque unde esse nisi quod facilis laudantium quibusdam!
          pLorem ipsum dolor sit amet consectetur adipisicing elit. Necessitatibus perferendis ullam fugit sint natus quis quaerat! Dolorum, debitis. Soluta totam molestias, dolorem neque unde esse nisi quod facilis laudantium quibusdam!
          pLorem ipsum dolor sit amet consectetur adipisicing elit. Necessitatibus perferendis ullam fugit sint natus quis quaerat! Dolorum, debitis. Soluta totam molestias, dolorem neque unde esse nisi quod facilis laudantium quibusdam!4</p>
        <div class="socialMedia">
        <h2>Gaysbook</h2>
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
.div-logo {
  display: flex;
  justify-content: center;
  align-items: center;
}
.logo {
  width: 180px;
  height: 200px;
}
/* Nav */
.nav {
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: rgb(255, 166, 0);
}
.ul-nav {
  list-style: none;
  display: flex;
}
/* Botones */
.btn-header a {
  text-decoration: none;
  background-color: rgb(255, 123, 0);
  color: rgb(255, 255, 255);
  padding: 10px;
  font-size: 20px;
  padding-left: 10px;
  padding-right: 10px;
}
.border-li1 a {
  border-top-left-radius: 10px;
  border-right: 1px solid black;
}
.border-li2 a {
  border-top-right-radius: 10px;
}
.border-li1 a:hover {
  border-top-left-radius: 10px;
}
.border-li2 a:hover {
  border-top-right-radius: 10px;
}
.sepBtn{
  border-right: 1px solid black;
}
.btn-header a:hover{
  background-color: rgb(222, 137, 58);
  color: rgb(0, 0, 0);
  padding: 10px;
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
  background-color: rgb(244, 167, 14);
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
  width: 97%;
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
  padding: 20px 0;
  height: 26em;
  border-left: rgb(56, 56, 56, 0.3) 2px solid;
}
.instaGram{
  width: 270px;  
  height: 400px; 
}
.div4-seccion2 {
  grid-row: 2;
  grid-column: 2;
  background-color: blue;
  padding: 10px;
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
  background-color: rgb(255, 0, 0);
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: justify;
  color: white;
  padding: 15px;
}
/* Footer */
.footer{
  background-color: black;
  display: flex;
  justify-content: center;
  align-items: center;
  color: azure;
  padding: 20px;
}
.footer:hover{
  color: rgb(110, 110, 110);
}
</style>
