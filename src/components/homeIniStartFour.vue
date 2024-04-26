<template>
  <div class="containerHaikyu">
    <div class="haikyu-info">
      <h2 id="title-info">Información de Haikyu!!</h2>
      <div class="description">
        <div class="detail-container">
          <p class="infocontainerTexto">"Haikyuu!!" es un popular manga y anime japonés que gira en torno al vóley masculino de preparatoria. 
            Fue creado por Haruichi Furudate. La serie se centra en Shoyo Hinata, un estudiante de secundaria con una
            estatura baja pero una gran pasión por el vóley. A pesar de sus limitaciones físicas, Hinata se une al equipo de 
            vóley de su escuela secundaria y se embarca en un viaje para convertirse en un jugador destacado.</p>
          <p class="infocontainerTexto">La trama sigue las experiencias de Hinata y sus compañeros de equipo mientras participan en diferentes
            torneos y compiten contra otros equipos poderosos. La serie no solo se enfoca en los partidos emocionantes,
            sino también en el desarrollo de los personajes, sus relaciones y cómo superan desafíos tanto dentro como fuera de la cancha.</p>
          <p class="infocontainerTexto">"Haikyuu!!" ha sido elogiado por su animación de alta calidad, su emocionante acción deportiva y sus personajes carismáticos y 
            bien desarrollados. Ha ganado una gran base de fanáticos tanto en Japón como en el extranjero desde su debut en 2012.</p>
          <p class="infocontainerTexto">Además del manga y el anime, "Haikyuu!!" ha inspirado películas, obras de teatro, videojuegos y una variedad 
            de productos de mercancía. Es considerado uno de los mejores trabajos en su género y ha contribuido significativamente 
            a aumentar el interés en el vóley en Japón y en todo el mundo.</p>
        </div>
        <div class="details">
          <div class="details-left">
            <div class="info-img--left">
              <img class="info-img--left-dimension" src="../assets/21406d787b688124db6945b3f1fa5e1c-removebg-preview.png" alt="">
            </div>
            <div class="details-right">
              <br>
              <br>
              <br>
                <p><strong class="info-titles--font">Título:</strong> Haikyu!!</p>
                <p><strong class="info-titles--font">Género</strong></p>
                <p class="info-titles--font">Deporte, comedia, drama, shonen</p>
                <p><strong class="info-titles--font">Estudio de animación:</strong> </p>
                <p class="info-titles--font">Production I.G</p>
                <p><strong class="info-titles--font">Director:</strong> Susumu Mitsunaka</p>
                <p><strong class="info-titles--font">Año de emisión:</strong> 2014 - 2020</p>
                <p><strong class="info-titles--font">Número de temporadas:</strong> 4</p>
                <p><strong class="info-titles--font">Número de episodios:</strong> 85</p>
                <p><strong class="info-titles--font">Manga original:</strong></p>
                <p class="info-titles--font"> Escrito por Haruichi Furudate</p>
                <p><strong class="info-titles--font">Fecha de publicación del manga:</strong></p>
                <p class="info-titles--font">20 de febrero de 2012 - presente</p>
                <p><strong class="info-titles--font">Editorial del manga:</strong> Shueisha</p>
            </div>
            <div class="info-img--right"> 
              <img class="info-img--right-dimension" src="../assets/efre-removebg-preview.png" alt="">
            </div>
        </div>
      </div>
    </div>
    <h2 id="title-info--map"> Mapa</h2>
    <div class="iframe-container">
      <br>
        <iframe class="maps" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3241.5929918232378!2d139.7414604751261!3d35.66239817259337!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x60188b7dabe6e4c7%3A0x2e63cece78e68104!2sShueisha%20Manga%20Art%20Heritage!5e0!3m2!1ses-419!2sco!4v1706982028625!5m2!1ses-419!2sco" 
        width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HaikyuInfo'
}
</script>

<style scoped>
.containerHaikyu {
  flex-wrap: wrap;
  font-size: 15px;
  display: flex;
  justify-content: center;
  background-color: rgb(255, 123, 0);
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  padding: 10px;
  padding-top: 1.5em;
}
.haikyu-info {
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin: 2px auto;
  border-radius: 10px;
  background-color: rgb(255, 255, 255);
  width: 80%;
  padding-top: 20px;
  margin-bottom: 0.8em;
}
#title-info {
  display: flex;
  justify-content: center;
  margin-top: 0.4em;
  margin-bottom: 1em;
  font-family: 'DIMISTRI', sans-serif;
  letter-spacing: 1px;
  color: #000000;
  font-size: 2.3em;
  text-align: center;
}
#title-info--map{
  display: flex;
  justify-content: center;  
  margin-top: 2em;
  font-family: 'DIMISTRI', sans-serif;
  letter-spacing: 1px;
  color: #000000;
  padding-bottom: 1em;
  font-size: 2.4em;
}
.infocontainerTexto {
  display: flex;
  justify-content: center;  
  text-align: center;
  align-items: center;
  margin-bottom: 20px;
  color: #000000;
  width: 95%;
  background-color: aqua;
}
.details{
  display: flex;
  justify-content: center;

}
.details-left{
  display: grid;
  grid-template-columns: 1f, 1f, 1f;
  grid-auto-rows: 1f;
  padding: 0;
  width: 90%;
  background-color: rgb(247, 242, 213);
  border-radius: 50% 50% 50% 50%;
}
.info-img--left{
  display: flex;
  justify-content: center;
  align-items: center;
  grid-column: 1;
  grid-row: 1;
  padding: 0;
}
.details-right{
  grid-column: 2;
  grid-row: 1;
  padding: 0;
}
.info-img--right{
  grid-column: 3;
  grid-row: 1;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
}

.info-img--left-dimension{
  height: auto;
  width: 100%;
}
.info-img--right-dimension{
  height: auto;
  width: 100%;
}
.details p {
  margin-bottom: 10px;
  color: #000000;
  padding-left: 40px;
}
.details strong {
  padding-right: 5px;
}
.details strong {
  font-weight: bold;
}
.detail-container {
  padding-bottom: 2em;
  padding-left: 5%;
}
.info-titles--font{
  color: #ff9900;
}
.iframe-container {
  position: relative;
  width: 100%;
  padding-bottom: 40%;
  border: solid 1px rgb(255, 123, 0, 0.1);}
.maps {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border: 0;
}
@media only screen and (min-width: 100px) and (max-width: 750px) {
.detail-container{
  width: 95%;
  text-align: justify;
  /* background-color: rgb(180, 24, 224); */
}
.infocontainerTexto{
  width: 100%;
}
.info-img--right-dimension{
  display: none;
}
.info-img--left-dimension{
  display: none;
}
.details-left{
  background-color: rgb(247, 242, 213);
  padding: 0;
  width: 100%;
  height: 80vh;
  border-radius: 60% 60% 60% 60%;
}
.details-right{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  grid-column: 2;
  grid-row: 1;
  padding: 0;
  margin-bottom: 4em;
  margin-right: 5em;
  width: 90%;
  font-size: 12px;
}
.iframe-container {
  position: relative;
  height: 70vh;
  width: 100%;
  padding-bottom: 40%;
  border: solid 1px rgb(255, 123, 0, 0.1);}
}
#title-info {
  display: flex;
  justify-content: center;
  margin-top: 0.4em;
  margin-bottom: 1em;
  font-family: 'DIMISTRI', sans-serif;
  letter-spacing: 1px;
  color: #000000;
  font-size: 2em;
  text-align: center;
}
</style>

