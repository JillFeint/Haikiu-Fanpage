<template>
  <div class="teamFull">
    <div class="topTitle">
      <h2 class="titleTop">Equipo de Haikyu</h2></div>
    <div class="teamFourOrden">
    <div class="teamFourOne">
    <!-- Jugador 1 -->
    <div class="teamMember">
      <div class="memberImage">
        <img src="../assets/1.jpeg" alt="Player 1">
      </div>
      <div class="memberDetails">
        <h3 class="memberOne">Shoyo Hinata</h3>
        <p>Posición: Colocador</p>
        <p>Altura: 162.8 cm</p>
        <p>Peso: 51 kg</p>
      </div>
    </div>
    <!-- Jugador 2 -->
    <div class="teamMember">
      <div class="memberImage">
        <img src="../assets/1.jpeg" alt="Player 2">
      </div>
      <div class="memberDetails">
        <h3>Tobio Kageyama</h3>
        <p>Posición: Colocador</p>
        <p>Altura: 180.6 cm</p>
        <p>Peso: 66 kg</p>
      </div>
    </div>
    <!-- Jugador 3 -->
    <div class="teamMember">
      <div class="memberImage">
        <img src="../assets/3.jpeg" alt="Player 3">
      </div>
      <div class="memberDetails">
        <h3 class="memberThree">Daichi Sawamura</h3>
        <p>Posición: Capitán / Levantador</p>
        <p>Altura: 179.6 cm</p>
        <p>Peso: 70 kg</p>
      </div>
    </div>
    <!-- Jugador 4 -->
    <div class="teamMember">
      <div class="memberImage">
        <img src="../assets/4.jpeg" alt="Player 4">
      </div>
      <div class="memberDetails">
        <h3>Koshi Sugawara</h3>
        <p>Posición: Levantador</p>
        <p>Altura: 176.8 cm</p>
        <p>Peso: 64 kg</p>
      </div>
    </div>
    </div>
    <div class="teamFourOne2">
    <!-- Jugador 5 -->
    <div class="teamMember">
    <div class="memberImage">
      <img src="../assets/5.jpeg" alt="Player 5">
    </div>
    <div class="memberDetails">
      <h3>Koshi Sugawara</h3>
      <p>Posición: Levantador</p>
      <p>Altura: 176.8 cm</p>
      <p>Peso: 64 kg</p>
    </div>
    </div>
    <!-- Jugador 6 -->
    <div class="teamMember">
    <div class="memberImage">
      <img src="../assets/6.jpeg" alt="Player 6">
    </div>
    <div class="memberDetails">
      <h3>Koshi Sugawara</h3>
      <p>Posición: Levantador</p>
      <p>Altura: 176.8 cm</p>
      <p>Peso: 64 kg</p>
    </div>
    </div>
    <!-- Jugador 7 -->
    <div class="teamMember">
    <div class="memberImage">
      <img src="../assets/7.jpeg" alt="Player 7">
    </div>
    <div class="memberDetails">
      <h3>Koshi Sugawara</h3>
      <p>Posición: Levantador</p>
      <p>Altura: 176.8 cm</p>
      <p>Peso: 64 kg</p>
    </div>
    </div>
    <!-- Jugador 8 -->
    <div class="teamMember">
    <div class="memberImage">
      <img src="../assets/1.jpeg" alt="Player 8">
    </div>
    <div class="memberDetails">
      <h3>Koshi Sugawara</h3>
      <p>Posición: Levantador</p>
      <p>Altura: 176.8 cm</p>
      <p>Peso: 64 kg</p>
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
  padding: 25px;
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
