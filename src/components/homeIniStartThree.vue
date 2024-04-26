<template>
  <div class="galleryGlobalContainer3">
    <div class="calendar">
      <div class="logosTop"><img class="logoLeft" src="../assets/stickerclean.png" alt="">
        <h1 class="titleCalen">Calendario de Karasuno!!</h1>
        <img class="logoRight" src="../assets/loguito2.png" alt="">
      </div>
      <div class="buttonsCalendar">
        <button class="buttonCalendar" @click="clickChange('months')">Entrenamiento proximos</button>
        <button class="buttonCalendar" @click="clickChange('showTwo')">Partidos que se aproximan</button>
      </div>
      <div class="months"  v-show="calendarShow">
        <!-- Aquí se generan los meses y los días automáticamente con JavaScript -->
      </div>
      <div class="showTwo" v-show="showTwoShow">
        <ul class="match-list">
          <li>
            <span class="match-date">Enero 10, 2024</span> - Haikui vs. Equipo A
          </li>
          <li id="otherColor">
            <span class="match-date" id="otherColor">Febrero 2, 2024</span> - Haikui vs. Equipo B
          </li>
          <li>
            <span class="match-date">Marzo 15, 2024</span> - Haikui vs. Equipo C
          </li>
          <li id="otherColor">
            <span class="match-date" id="otherColor">Abril 5, 2024</span> - Haikui vs. Equipo D
          </li>
          <li>
            <span class="match-date">Mayo 20, 2024</span> - Haikui vs. Equipo E
          </li>
          <li id="otherColor">
            <span class="match-date" id="otherColor">Junio 8, 2024</span> - Haikui vs. Equipo F
          </li>
          <li>
            <span class="match-date">Julio 12, 2024</span> - Haikui vs. Equipo G
          </li>
          <li id="otherColor">
            <span class="match-date" id="otherColor">Agosto 3, 2024</span> - Haikui vs. Equipo H
          </li>
          <li>
            <span class="match-date">Septiembre 18, 2024</span> - Haikui vs. Equipo I
          </li>
          <li id="otherColor">
            <span id="otherColor" class="match-date">Octubre 10, 2024</span> - Haikui vs. Equipo J
          </li>
          <li>
            <span class="match-date">Noviembre 5, 2024</span> - Haikui vs. Equipo K
          </li>
          <li id="otherColor">
            <span class="match-date" id="otherColor">Diciembre 22, 2024</span> - Haikui vs. Equipo L
          </li>
        </ul>
      </div>
    </div>
</div>
</template>
<script>
export default {
  data() 
  {
    return {
    calendarShow: true,
    showTwoShow: false,      
    };
  },
  methods: {
    clickChange(componentName) {
      this.calendarShow = false;
      this.showTwoShow = false;  
      switch (componentName) {
        case 'months':
        this.calendarShow = true;
          break;
        case 'showTwo':
          this.showTwoShow = true;
          break;
      }
    }
  },
  mounted() {
    const monthsContainer = this.$el.querySelector('.months');
    const months = [
      'Enero', 'Febrero', 'Marzo', 'Abril', 'Mayo', 'Junio',
      'Julio', 'Agosto', 'Septiembre', 'Octubre', 'Noviembre', 'Diciembre'
    ];
    // Define los días que deseas resaltar para cada mes
    const highlightedDays = {
      'Enero': [1, 15, 28],
      'Febrero': [14, 7, 11],
      'Marzo': [8, 20, 21, 22, 23, 28],
      'Junio': [8, 10, 14, 15, 16, 20],
      'Julio': [1, 3, 5, 8, 20, 22, 26 , 28],
      'Agosto': [1, 3, 5, 8, 20, 22, 26 , 28],
      'Septiembre': [8, 20],
      'Noviembre': [8, 12, 13, 15, 16, 20],
      
      // Agrega más meses y días según lo necesites
    };

    months.forEach(month => {
      const monthDiv = document.createElement('div');
      monthDiv.classList.add('month');
      monthDiv.innerHTML = `<h2>${month}</h2>`;
      
      const daysDiv = document.createElement('div');
      daysDiv.classList.add('days');
      
      for (let i = 1; i <= 31; i++) {
        const dayDiv = document.createElement('div');
        dayDiv.classList.add('day');
        dayDiv.textContent = i;

        // Verifica si el día debe tener un color diferente
        if (highlightedDays[month] && highlightedDays[month].includes(i)) {
          dayDiv.classList.add('highlighted');
        }

        daysDiv.appendChild(dayDiv);
      }
      
      monthDiv.appendChild(daysDiv);
      monthsContainer.appendChild(monthDiv);
    });
  }
}
</script>

<style>
/* Estilo adicional para los días resaltados */
.highlighted {
  background-color: rgb(53, 54, 68);
  color: #fff;
}
.galleryGlobalContainer3 {
  display: flex;
  justify-content: center;
  font-family: Arial, sans-serif;
  background-color: rgb(255, 123, 0);
  margin: 0;
  padding: 0;
}
.buttonsCalendar{
  display:flex;
  justify-content: center;
  align-items: center;
  margin: 25px;
  gap:10px;
}
.buttonCalendar{
  padding: 10px;
  background-color: rgb(255, 123, 0);
  border: rgb(48, 48, 48, 0.3) solid 0.5px;
  font-size: 15px;
  border-radius: 5px;
  transition: background-color 0.3s;
  cursor: pointer;
  color: white;
}
.buttonCalendar:hover{
  background-color: rgba(255, 10, 6, 0.883);
}
.calendar {
  margin: 20px auto;
  background-color: #fff;
  border-radius: 10px;
  padding: 20px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  width: 60%;
  margin-top: 1.3em;
}
.logoLeft{
  width: auto;
  height: 4em;
}
.logoRight{
  width: auto; 
  height: 4em;
}
.logosTop{
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 40px
}
.titleCalen{
  text-align: center;
  color: #333;
  font-family: 'DIMISTRI', sans-serif;
}
.months {
  margin-top: 20px;
}

.month {
  margin-bottom: 20px;
}

.month h2 {
  background-color: rgb(255, 123, 0);
  color: #fff;
  padding: 10px;
  margin: 0;
  border-top-left-radius: 5px;
  border-top-right-radius: 5px;
}

.days {
  display: grid;
  grid-template-columns: repeat(7, 1fr);
}

.day {
  border: 1px solid #ccc;
  padding: 10px;
  text-align: center;
}
/* Partidos futuros */
.match-list {
  list-style: none;
  padding: 0;
}
/* Clase de los partidos en naranja*/
#otherColor{
  background-color: rgb(53, 54, 68);
  color: white;
}
.match-list li:hover{
  background-color: rgb(255, 123, 0);
}
.match-list li {
  margin-bottom: 20px;
  background-color: #ffffff;
  border-radius: 8px;
  padding: 15px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}
.match-date {
  font-weight: bold;
  color: #333333;
}
.match-opponent {
  margin-top: 5px;
  font-size: 16px;
  color: #666666;
}
.match-opponent:before {
  content: "- ";
}
.match-opponent a {
  text-decoration: none;
  color: #007bff;
}
.match-opponent a:hover {
  text-decoration: underline;
}
@media only screen and (min-width: 100px) and (max-width: 1024px) {
.galleryGlobalContainer3 {
  display: flex;
  justify-content: center;
  font-family: Arial, sans-serif;
  background-color: rgb(255, 123, 0);
  margin: 0;
  padding: 0;
}
.calendar {
  flex-direction: column;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #fff;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  width: 90%;
  margin-top: 1.3em;
}
.buttonsCalendar{
  position: relative;
  display:flex;
  justify-content: center;
  align-items: center;
  gap:5px;
  /* background-color: #007bff; */
  width: 100%;
}
.buttonCalendar{
  padding: 5px;
  background-color: rgb(255, 123, 0);
  border: rgb(48, 48, 48, 0.3) solid 0.5px;
  font-size: 12px;
  border-radius: 5px;
  transition: background-color 0.3s;
  cursor: pointer;
  color: white;
}
.buttonCalendar:hover{
  background-color: rgba(255, 10, 6, 0.883);
}

.logoLeft{
  display: none;
}
.logoRight{
display: none;
}
.logosTop{
  display: none;
}
.titleCalen{
  text-align: center;
  color: #333;
  font-family: 'DIMISTRI', sans-serif;
}
.months {
  margin-top: 20px;
}

.month {
  margin-bottom: 20px;
}

.month h2 {
  background-color: rgb(255, 123, 0);
  color: #fff;
  padding: 10px;
  margin: 0;
  border-top-left-radius: 5px;
  border-top-right-radius: 5px;
}

.days {
  position: relative;
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  width: 90%;
}

.day {
  border: 1px solid #ccc;
  padding: 10px;
  text-align: center;
}
/* Partidos futuros */
.match-list {
  list-style: none;
  padding: 0;
}
/* Clase de los partidos en naranja*/
#otherColor{
  background-color: rgb(53, 54, 68);
  color: white;
}
.match-list li:hover{
  background-color: rgb(255, 123, 0);
}
.match-list li {
  margin-bottom: 20px;
  background-color: #ffffff;
  border-radius: 8px;
  padding: 15px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}
.match-date {
  font-weight: bold;
  color: #333333;
}
.match-opponent {
  margin-top: 5px;
  font-size: 16px;
  color: #666666;
}
.match-opponent:before {
  content: "- ";
}
.match-opponent a {
  text-decoration: none;
  color: #007bff;
}
.match-opponent a:hover {
  text-decoration: underline;
}
}
</style>