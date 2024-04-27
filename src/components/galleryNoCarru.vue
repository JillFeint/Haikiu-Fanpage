<template>
  <div class="div-btnsSec3">
    <button @click="clickChangeToVideo('grid-container')" class="btnSec3"><span class="span-gallery">Fotos</span></button>
    <button @click="clickChangeToVideo('gridVideos')" class="btnSec3"><span class="span-gallery">Videos</span></button>
</div>
<div class="seccionG3">
<div class="grid-container" v-if="seccionG3Show">
  <img class="grid-item hoverAll" src="../assets/fotos/lo logramos.jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/descarga (1).jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/descarga.jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/Fly ✨.jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/G L O R I O S O ✨.jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/haikyuu.jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/Kageyama, Number Nine by aislingkiera.jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/Karasuno sticker (1).jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/Karasuno Volleyball Logo Sticker by itsboattime.jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/Team Karasuno Magnet.jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/Karasuno.jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/simbolitos chinos.jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/asa ッ (closed).jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/Atsumu.jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/descarga (4).jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/descarga (3).jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/descarga (2).jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/Haikyuuttt.jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/DESENHANDO HINATA SHOYO DE HAIKYUU.jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/Haikyuu ONE-SHOTS [edición 2020] - Nishinoya Yū.jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/letras rusas.jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/Wallpapers Haikyuu.jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/Реакция haikyuu _ волейбол.jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/Pegatinas_ Haikyuu.jpg">
  <img class="grid-item hoverAll" src="../assets/fotos/_3.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/_33.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/4b1d0086-dacf-44ef-a9d6-9013d0b0c983.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/82f2a123-26f5-4721-9912-fc07ce53ba7f.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/37848cc9-1a28-44a1-bba0-d85aafcb165e.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/28876200-8f05-4688-8f1a-12c02d5226e2.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/alosed) (1).jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/asa closed).jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/asaclosed) (1).jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/asaclosed).jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/cara.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/dc762ac4-74c2-448f-becb-d0cf7ba59c27.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/h a i k y u u.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/Haikyuu Wallpapers 30.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/hayyba.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/kageyama tobio  hiromizu.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/Kageyama tobio.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/Las mejores versiones de HaikyuuHappy Haikyuu.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/My pretty boy Akaashi keiji.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/Nishnoya.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/noya.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/Oiwaka Tooru.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/rojo123.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/Segundos (Oikawa x Reader).jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/ShoyoHinata.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/Sweatshirt Tendō.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/Tanaka.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/Your Haikyuu Life.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/Your Haikyuu Lover.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/Yuu Nishinoya Icon.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/espaldaa.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/circulo22.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/123cancer.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/icons hinata.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/kurooo.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/123rojoo.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/pandalinn.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/asahi 123.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/keishi ukani.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/interest 3.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/kenma1.jpeg">
  <img class="grid-item hoverAll" src="../assets/fotos/interes 245.jpeg">
  
  <!-- <img class="grid-item hoverAll" src="../assets/fotos">
  <img class="grid-item hoverAll" src="../assets/fotos">
  <img class="grid-item hoverAll" src="../assets/fotos">
  <img class="grid-item hoverAll" src="../assets/fotos"> -->
    
  </div>
  <div class="gridVideos" v-if="seccionVideosShow">
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/Lv59h1zDl-U" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/5f9U9a6zBD8" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/AH-nw5EYOYw" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/LAo7Q3nnYZQ" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/ReiuuLolkHk" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/zOQGr0K75kY" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/xFQzzdUSV7k" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/cAlg-4YgEUE" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/Lv59h1zDl-U" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/5f9U9a6zBD8" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/AH-nw5EYOYw" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/LAo7Q3nnYZQ" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/ReiuuLolkHk" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/zOQGr0K75kY" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/xFQzzdUSV7k" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/cAlg-4YgEUE" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/Lv59h1zDl-U" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/5f9U9a6zBD8" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/AH-nw5EYOYw" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/LAo7Q3nnYZQ" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/ReiuuLolkHk" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/zOQGr0K75kY" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/xFQzzdUSV7k" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/cAlg-4YgEUE" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/Lv59h1zDl-U" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/5f9U9a6zBD8" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/AH-nw5EYOYw" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/LAo7Q3nnYZQ" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/ReiuuLolkHk" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/zOQGr0K75kY" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/xFQzzdUSV7k" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/cAlg-4YgEUE" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/Lv59h1zDl-U" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/5f9U9a6zBD8" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/AH-nw5EYOYw" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/LAo7Q3nnYZQ" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/ReiuuLolkHk" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/zOQGr0K75kY" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/xFQzzdUSV7k" frameborder="0" allowfullscreen></iframe>
    <iframe class="grid-itemVds hoverAll" width="300" height="300" src="https://www.youtube.com/embed/cAlg-4YgEUE" frameborder="0" allowfullscreen></iframe>
  </div>
</div>
</template>
<script>
export default {
data() 
{
return {
seccionG3Show: true,
seccionVideosShow: false,      
};
},
methods: {
clickChangeToVideo(componentName) {
  this.seccionG3Show = false;
  this.seccionVideosShow = false;  
  switch (componentName) {
    case 'grid-container':
      this.seccionG3Show = true;
      break;
    case 'gridVideos':
      this.seccionVideosShow = true;
      break;
  }
}
},
}
</script>
<style>
.seccionG3 {
height: 100%;
width: 74%;
background-color: rgb(53, 54, 68);
box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.5);
color: white;
padding: 1em 0;
padding-left: 1em;
padding-right: 1em;
margin: 1em 0;
overflow-y: auto;
}
/* Estilos específicos para la barra de desplazamiento en navegadores WebKit en navegadores basados en WebKit (como Google Chrome y Safari)*/
.seccionG3::-webkit-scrollbar {
width: 0.5em; /* Ancho de la barra de desplazamiento */
}
.seccionG3::-webkit-scrollbar-thumb {
background-color: transparent; /* Color del pulgar de la barra de desplazamiento */
}
.seccionG3::-webkit-scrollbar-track {
background-color: transparent; /* Color de la pista de la barra de desplazamiento */
}
/* Estilos específicos para la barra de desplazamiento en navegadores Firefox */
.seccionG3 {
scrollbar-width: thin; /* Ancho de la barra de desplazamiento */
scrollbar-color: transparent transparent; /* Color del pulgar y la pista de la barra de desplazamiento */
}
.grid-container {
display: grid;
grid-template-columns: repeat(auto-fill, 220px);
gap: 20px;
height: 34em;
justify-content: center;
margin: 0 auto;
overflow-y: auto;
}
.grid-item {
cursor: pointer;
transition: filter 0.3s ease-in-out;
width: 220px;
height: 170px;
object-fit: cover;
background-color: lightgray;
}
.gridVideos{
display: grid;
grid-template-columns: repeat(auto-fill, 300px);
gap: 20px;
height: 40em;
justify-content: center;
align-items: center;
overflow-y: auto;
}
.grid-itemVds {
cursor: pointer;
transition: filter 0.3s ease-in-out;
width: 300px;
height: 200px;
object-fit: cover;
background-color: lightgray;
}
/* Agrega estos estilos para el efecto de elevación y descripción */
.hoverAll {
position: relative;
}
.hoverAll:hover {
filter: brightness(80%); /* Puedes ajustar este valor según tus preferencias */
transform: translateY(-5px);
}
.hoverAll::after {
content: "Descripción de la imagen";
font-size: 13px;
position: absolute;
bottom: 0;
left: 0;
width: 100%;
padding: 10px;
visibility: visible; /* Ajusta esta línea */
background-color: rgba(0, 0, 0, 0.8);
color: white;
opacity: 0.9;
transition: visibility 0s, opacity 0.3s ease-in-out;
}
.hoverAll:hover::after {
opacity: 1; /* Agrega esta línea para garantizar que la opacidad sea 1 al hacer hover */
}
.div-btnsSec3 {
display: flex;
justify-content: center;
gap: 1.5em;
}
.btnSec3 {
background-color: rgb(255, 123, 0);
color: white;
border: none;
padding: 11px 20px;
display: inline-block;
font-size: 20px;
/* font-weight: 600; */
font-family: 'DIMIS___', sans-serif;
letter-spacing: 1.5px; /* Esto es para el espacio entre letras */
width: 120px;
text-transform: uppercase;
cursor: pointer;
transform: skew(-21deg);
}
.span-gallery {
display: inline-block;
transform: skew(21deg);
}
.btnSec3::before {
content: '';
position: absolute;
top: 0;
bottom: 0;
right: 100%;
left: 0;
background-color: rgba(255, 10, 6, 0.883);
opacity: 0;
z-index: -1;
transition: all 0.5s;
}
.btnSec3:hover::before {
left: 0;
right: 0;
opacity: 1;
}
@keyframes ripple {
0% {
box-shadow: 0 0 0 0 rgba(255, 255, 255, 0.1), 0 0 0 20px rgba(255, 255, 255, 0.1), 0 0 0 20px rgba(255, 255, 255, 0.1), 0 0 0 60px rgba(255, 255, 255, 0.1);
}

100% {
box-shadow: 0 0 0 20px rgba(255, 255, 255, 0.1), 0 0 0 40px rgba(255, 255, 255, 0.1), 0 0 0 60px rgba(255, 255, 255, 0.1), 0 0 0 80px rgba(255, 255, 255, 0);
}
}
.btnsSec3 {
display: flex;
gap: 1em;
}
/* .btnSec3 {
text-decoration: none;
color: aliceblue;
background-color: rgb(255, 123, 0);
padding: 7px;
font-size: 21px;
transition: 1s;
transform: skewX(-15deg);
border: none;
box-shadow: 4px 4px 0 black;
border-right: 1px solid black;
animation: color_anim 1s infinite 0.2s;
margin: 0.3em;
z-index: 9999;
} */
</style>
