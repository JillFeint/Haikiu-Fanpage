<template>
  <div class="galleryGlobalContainer">
    <div class="boxContainer1">
    <div class="divContainer1 hoverAll">
      <img class="1 sizeAll" src="../assets/1.jpeg" alt="">
    </div>
    <div class="divContainer2 hoverAll">
      <img class="2 sizeAll" src="../assets/2.jpeg" alt="">
    </div>
    <div class="divContainer3 hoverAll">   
      <img class="3 sizeAll" src="../assets/3.jpeg" alt="">
    </div>
    <div class="divContainer4 hoverAll">   
      <img class="4 sizeAll" src="../assets/4.jpeg" alt="">
    </div>
    <div class="divContainer5 hoverAll">   
      <img class="5 sizeAll" src="../assets/5.jpeg" alt="">
    </div>
    <div class="divContainer6 hoverAll">
      <img class="6 sizeAll" src="../assets/6.jpeg" alt="">
    </div>
    <div class="divContainer7 hoverAll">
      <img class="7 sizeAll" src="../assets/7.jpeg" alt="">
    </div>
    <div class="divContainer8 hoverAll">   
      <img class="8 sizeAll" src="../assets/8.png" alt="">
    </div>
    <div class="divContainer9 hoverAll">   
      <img class="9 sizeAll" src="../assets/9.png" alt="">
    </div>
    <div class="divContainer10 hoverAll">   
      <img class="10 sizeAll" src="../assets/10.jpeg" alt="">
    </div>
    </div>
  </div>
</template>

<script>

</script>


<style>
.galleryGlobalContainer{
padding: 10px;
}
.divContainer1 {
  grid-column: 1;
  grid-row: 1;
}
.divContainer2 {
  grid-column: 2;
  grid-row: 2;
}
.divContainer3 {
  grid-column: 3;
  grid-row: 3;
}
.divContainer4 {
  grid-column: 4;
  grid-row: 4;
}
.divContainer5 {
  grid-column: 5;
  grid-row: 5;
}
.divContainer6 {
  grid-column: 1;
  grid-row: 2;
}
.divContainer7 {
  grid-column: 4;
  grid-row: 5;
}
.divContainer8 {
  grid-column: 5;
  grid-row: 1;
}
.divContainer9 {
  grid-column: 1;
  grid-row: 5;
}
.divContainer10 {
  grid-column: 2;
  grid-row: 5;
}
.boxContainer1{
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr 1f 1fr;
  width: 100%;
  height: 45em;
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.5);
  overflow: hidden;
  grid-gap: 20px;
  padding: 20px;
  background-color: rgb(250, 108, 0);
}
.hoverAll {
  position: relative; /* Asegura que el ::after sea relativo a este elemento */
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.5);
  box-sizing: border-box;
  height: 100%; 
  width: 100%;
  max-height: 8em;
  max-width: 9.5em;
  cursor: pointer;
  transition: transform 0.3s ease-in-out;
}
.hoverAll:hover{
  transform: translateY(-10px);
}
.hoverAll::after {
  box-sizing: border-box; /* Incluye el padding y el borde en el ancho total */
  content: "Descripción de la imagen";
  font-size: 13px;
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  padding: 20px;
  visibility: hidden;
  background-color: rgba(0, 0, 0, 0.3);
  overflow: hidden;
  color: azure;
}
.hoverAll:hover::after {
  visibility: visible; /* Hace visible el texto al hacer hover */
}
/* Img */
.sizeAll{
  box-sizing: border-box;
  height: 100%;
  width: 100%;
  object-fit: cover;
}
</style>