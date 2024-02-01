<template>
  <div class="teamFull">
    <h2>Equipo de Haikyu</h2>
    <div class="teamFourOne">
    <!-- Jugador 1 -->
    <div class="teamMember">
      <div class="memberImage">
        <img src="../assets/1.jpeg" alt="Player 1">
      </div>
      <div class="memberDetails">
        <h3>Shoyo Hinata</h3>
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
        <h3>Daichi Sawamura</h3>
        <p>Posición: Capitán <br>/ Levantador</p>
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
  <div class="teamFourOne">
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
      <img src="../assets/8.png" alt="Player 8">
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
  background-color: #ff9900;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}
.teamFourOne{
  background-color: rgb(56, 56, 56); 
  border-radius: 10px;
  box-shadow: 10px solid black;
  padding: 20px;
}
.teamFull h2 {
  font-size: 24px;
  color: #333;
  margin-bottom: 20px;
}

.teamMember {
  display: flex;
  margin-bottom: 20px;
}

.memberImage img {
  width: 120px;
  height: auto;
  border-radius: 50%;
}

.memberDetails {
  margin-left: 20px;
}

.memberDetails h3 {
  font-size: 20px;
  color: #000000;
  margin-bottom: 10px;
}

.memberDetails p {
  font-size: 16px;
  color: aliceblue;
  margin-bottom: 5px;
}
</style>
