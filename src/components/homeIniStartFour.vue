<template>
  <div class="containerHaikyu">
  <div class="haikyu-info">
    <h2 class="title">Información de Haikyu!!</h2>
    <div class="description">
      <p>Haikyu!! es un anime japonés que gira en torno al deporte del voleibol. La historia sigue a Shoyo Hinata, un estudiante de secundaria con una pasión ardiente por el voleibol, quien se une al equipo de su escuela con el objetivo de convertirse en el mejor jugador. A lo largo de la serie, Hinata enfrenta desafíos, trabaja en equipo y lucha por alcanzar sus sueños.</p>
      <p>El anime se caracteriza por su emocionante acción en la cancha, sus intensos partidos de voleibol y la profundidad de sus personajes. Además del aspecto deportivo, también explora temas como la amistad, la superación personal y la rivalidad.</p>
    </div>
    <div class="details">
      <p><strong>Título:</strong> Haikyu!!</p>
      <p><strong>Género:</strong> Deporte, Comedia, Drama, Escolar, Shonen</p>
      <p><strong>Estudio de animación:</strong> Production I.G</p>
      <p><strong>Director:</strong> Susumu Mitsunaka</p>
      <p><strong>Año de emisión:</strong> 2014 - 2020</p>
      <p><strong>Número de temporadas:</strong> 4</p>
      <p><strong>Número de episodios:</strong> 85</p>
      <p><strong>Manga original:</strong> Escrito por Haruichi Furudate</p>
      <p><strong>Editorial del manga:</strong> Shueisha</p>
      <p><strong>Fecha de publicación del manga:</strong> 20 de febrero de 2012 - presente</p>
    </div>
    <div class="iframe-container">  
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
.containerHaikyu{
  display: flex;
  justify-content: center;
  background-color: #ff9900;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  padding: 10px;
}
.haikyu-info {
  max-width: 100%;
  margin: 0;
  padding: 50px;
  border-radius: 10px;
  background-color: rgb(53, 54, 68);
  width: 75%;
}
.title {
  text-align: center;
  margin-bottom: 10px;
}
.description {
  margin-bottom: 20px;
}
.description p {
  margin-bottom: 20px;
  color: #ccc;
}
.details p {
  margin-bottom: 10px;
  color: #ccc;
}
.details strong {
  font-weight: bold;
}
.iframe-container {
  position: relative;
  width: 100%;
  padding-bottom: 40%;
}
.maps {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border: 0;
}
</style>
