<template>
  <div class="teamFull">
    <div class="topTitle">
      <h2 class="titleTop">Equipo de Haikyu</h2></div>
    <div class="teamFourOrden">
    <div class="teamFourOne">
    <!-- Jugador 1 -->
    <div class="teamMember">
      <div class="memberImage">
        <img src="../assets/jugadores/Yū Nishinoya.jpeg" alt="Player 1">
      </div>
      <div class="memberDetails">
        <h3 class="memberOne">Yū Nishinoya</h3>
        <p>Posición: Libero</p>
        <p>Altura: 159,3 cm</p>
        <p>Peso: 51,1 kg</p>
        <p>Numero: 4</p>
        <p>Edad: 17</p>
      </div>
    </div>
    <!-- Jugador 2 -->
    <div class="teamMember">
      <div class="memberImage">
        <img src="../assets/jugadores/Ryūnosuke Tanaka.jpeg" alt="Player 2">
      </div>
      <div class="memberDetails">
        <h3>Ryūnosuke Tanaka</h3>
        <p>Posición: Punta Receptor</p>
        <p>Altura: 177,2 cm</p>
        <p>Peso: 68,8 kg</p>
        <p>Numero: 5</p>
        <p>Edad: 16</p>
      </div>
    </div>
        <!-- Jugador 3 -->
        <div class="teamMember">
    <div class="memberImage">
      <img src="../assets/jugadores/Chikara Ennoshita.jpeg" alt="Player 3">
    </div>
    <div class="memberDetails">
      <h3>Chikara Ennoshita</h3>
      <p>Posición: Punta receptor</p>
      <p>Altura: 175,4 cm</p>
      <p>Peso: 66,4 kg</p>
      <p>Numero: 6</p>
      <p>Edad: 18</p>
    </div>
    </div>
    <!-- Jugador 4 -->
    <div class="teamMember">
      <div class="memberImage">
        <img src="../assets/jugadores/Asahi Azumane.jpeg" alt="Player 4">
      </div>
      <div class="memberDetails">
        <h3>Asahi Azumane</h3>
        <p>Posición: Punta receptor</p>
        <p>Altura: 184,7 cm</p>
        <p>Peso: 75,2 kg</p>
        <p>Numero: 3</p>
        <p>Edad: 18</p>
      </div>
    </div>
    <!-- Jugador 5 -->
    <div class="teamMember">
      <div class="memberImage">
        <img src="../assets/jugadores/Daichi Sawamura.jpeg" alt="Player 5">
      </div>
      <div class="memberDetails">
        <h3>Daichi Sawamura</h3>
        <p>Posición: Capitan/Opuesto</p>
        <p>Altura: 17,.8 cm</p>
        <p>Peso: 70,1 kg</p>
        <p>Numero: 1</p>
        <p>Edad: 18</p>
      </div>
    </div>
    </div>
    <div class="teamFourOne2">
    <!-- Jugador 6 -->
    <div class="teamMember">
    <div class="memberImage">
      <img src="../assets/jugadores/Tobio Kageyama.jpeg" alt="Player 6">
    </div>
    <div class="memberDetails">
      <h3>Tobio Kageyama</h3>
      <p>Posición: Armador</p>
      <p>Altura: 180,6 cm</p>
      <p>Peso: 66,3 kg</p>
      <p>Numero: 9</p>
      <p>Edad: 15</p>
    </div>
    </div>
    <!-- Jugador 7 -->
    <div class="teamMember">
    <div class="memberImage">
      <img src="../assets/jugadores/Shōyō Hinata.jpeg" alt="Player 7">
    </div>
    <div class="memberDetails">
      <h3>Shōyō Hinata</h3>
      <p>Posición: Bloqueador Central</p>
      <p>Altura: 162,8 cm</p>
      <p>Peso: 51,9 kg</p>
      <p>Numero: 10</p>
      <p>Edad: 16</p>
    </div>
    </div>
    <!-- Jugador 8 -->
    <div class="teamMember">
    <div class="memberImage">
      <img src="../assets/jugadores/Kei Tsukishima.jpeg" alt="Player 8">
    </div>
    <div class="memberDetails">
      <h3>Kei Tsukishima</h3>
      <p>Posición: Bloqueador Central</p>
      <p>Altura: 188.3 cm</p>
      <p>Peso: 68,4 kg</p>
      <p>Numero: 16</p>
      <p>Edad: 17</p>
    </div>
    </div>
        <!-- Jugador 9 -->
        <div class="teamMember">
    <div class="memberImage">
      <img src="../assets/jugadores/Tadashi Yamaguchi.jpeg" alt="Player 9">
    </div>
    <div class="memberDetails">
      <h3>Tadashi Yamaguchi</h3>
      <p>Posición: Central/Sacador de apoyo</p>
      <p>Altura: 179,5 cm</p>
      <p>Peso: 63 kg</p>
      <p>Numero: 12</p>
      <p>Edad: 15</p>
    </div>
    </div>
    <!-- Jugador 10 -->
    <div class="teamMember">
    <div class="memberImage">
      <img src="../assets/jugadores/Kōshi Sugawara.jpeg" alt="Player 10">
    </div>
    <div class="memberDetails">
      <h3>Koshi Sugawara</h3>
      <p>Posición: Armador suplente</p>
      <p>Altura: 174,3 cm</p>
      <p>Peso: 63,5 kg</p>
      <p>Numero: 2</p>
      <p>Edad: 18</p>
    </div>
    </div>
    </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isVisibleShow2: false,
    };
  },
};
</script>

<style scoped>
/* Estilos específicos para el componente del equipo */
.teamFull {
  display: flex;
  flex-direction: column;
  background-color: #ff9900;
  padding: 20px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}
.topTitle{
  display: flex;
  justify-content: center;
}
.titleTop{
  color: #000000;
}
.titleTop:hover{
  color: white;
}
.teamFourOrden{
  display: flex;
  justify-content: center;
}
.teamFourOne{
  background-color: rgb(53, 54, 68);
  border-top-left-radius: 10px;
  border-bottom-left-radius: 10px;
  box-shadow: 10px solid black;
  padding: 30px;
}
.teamFourOne2{
  background-color: rgb(53, 54, 68);  
  border-top-right-radius: 10px;
  border-bottom-right-radius: 10px;
  box-shadow: 10px solid black;
  padding: 33px;
}
.teamFull h2 {
  font-size: 24px;
  margin-bottom: 2px;
  background-color: rgb(255, 123, 0);
  padding: 7px;
  margin-bottom: 10px;
  width: 20%;
  border-radius: 10px;
  border: 1px solid rgb(0, 0, 0);
}
.teamMember {
  display: flex;
  margin-bottom: 50px;
}
.memberImage img {
  width: 170px;
  height: auto;
  border-radius: 60%;
}
.memberDetails {
  margin-left: 20px;
}
.memberDetails h3 {
  font-size: 20px;
  background-color: rgb(255, 123, 0);
  margin-bottom: 10px;
}
.memberThree{
  width: 7.7em;
}
.memberOne{
  width: 5.9em;
}
.memberDetails p {
  font-size: 16px;
  color: aliceblue;
  margin-bottom: 5px;
  width: 100%;
}
</style>
