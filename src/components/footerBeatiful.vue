<template>
  <div class="footerBeatifulBig">
    <div class="footerBeatifulLogo">
      <img class="footerBeatifulImg" src="../assets/logoCorto.png" alt="">
    </div>
    <div class="footerBeatifulTexto">
      &copy; Moncada, Ballesteros & Jill Angel LLC, a subsidiary of Compas del codigo de hierro, 2024 Inc. All Rights Reserved.
    </div>
    <div class="footerBeatifulBotones">
      <div class="footerBeatifulBotonPoliticas footerBeatifulSpace">
        <buttom class="footerBeatifulEnlacePoliticas footerBeatifulEnlaces ">Políticas</buttom>
      </div>
      <div class="footerBeatifulBotonInformacion footerBeatifulSpace">
        <buttom class="footerBeatifulEnlaceInformacion footerBeatifulEnlaces">Informacion</buttom>
      </div>
      <div class="footerBeatifulBotonPrivacidad footerBeatifulSpace">
        <buttom class="footerBeatifulEnlacePrivacidad footerBeatifulEnlaces">Privacidad</buttom>
      </div>
    </div>
  </div>
</template>

<script>

</script>

<style>
.footerBeatifulBig{
  width: 100%;
  height: auto;
  background-color: rgb(53, 54, 68);
  display: flex;
  align-items: center;
  flex-direction: column;
  box-shadow: 0px -5px 5px rgba(0, 0, 0, 0.5);
}
.footerBeatifulLogo {
  display: flex;
  justify-content: center;
  background-color: rgba(31, 33, 70, 0);
  width: 100%;
}
.footerBeatifulImg {
  width: 11%;
  height: auto;
  margin: 1em 0;
  cursor: pointer;
}
.footerBeatifulImg:hover {
  /* background-color: chocolate; */
  transform: translatey(-5px); /* Cambia la distancia que se moverá */
}
.footerBeatifulTexto {
  background-color: rgba(31, 33, 70, 0);
  text-align: justify;
  text-justify: inter-word;
  width: auto;
  padding: 0 2em;
  padding-bottom: 2em;
  color: #fff;
  border-bottom: 1px solid black;
}
.footerBeatifulTexto:hover {
  color: rgb(255, 123, 0);
}
.footerBeatifulBotones {
  display: flex;
  margin-bottom: 1em;
  margin-top: 1em;
  /* background-color: blue; */
}
.footerBeatifulBotonPoliticas {
  display: flex;
  align-items: center;
  height: 15px;
  border-right: 1px solid black;
}
.footerBeatifulBotonInformacion {
  display: flex;
  align-items: center;
  height: 15px;
  border-right: 1px solid black;
}
.footerBeatifulBotonPrivacidad {
  display: flex;
  align-items: center;
  height: 15px;
}
.footerBeatifulEnlaces {
  color: #fff;
  padding: 7px 20px;
  border-radius: 5px;
  text-decoration: none;
  display: inline-block;
  cursor: pointer;
}
.footerBeatifulEnlaces:hover {
  background-color: rgb(255, 123, 0);
}
</style>