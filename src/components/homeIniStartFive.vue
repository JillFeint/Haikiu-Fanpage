<template>
  <div class="contactWeGlobal">
    <div class="contactWe1">
      <h2 id="fiveTitleContactanos">Contactanos</h2>
      <p class="pComponentContac">Por favor, envíanos tus consultas y comentarios. Estaremos encantados de ayudarte.</p>
      <form class="contactForm">
        <div  class="formGroup">
          <label class="pComponentContac" for="name">Nombre:</label>
          <input type="text" class="nameBackg" id="name" name="name" placeholder="Ingresa tu nombre">
        </div>
        <div class="formGroup">
          <label class="pComponentContac" for="email">Correo electrónico:</label>
          <input type="email" class="nameBackg" id="email" name="email" placeholder="Ingresa tu correo electrónico">
        </div>
        <div class="formGroup">
          <label class="pComponentContac" for="message">Mensaje:</label>
          <textarea id="message" name="message" rows="4" placeholder="Escribe aquí tu mensaje"></textarea>
        </div>
        <div class="btnSubmit">
          <button class="btnSubmit1" type="submit">Enviar mensaje</button>
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isVisibleShow5: false,
    };
  },
};
</script>
<style scoped>
.pComponentContac{
  color:#fff
}
#fiveTitleContactanos {
  display: flex;
  justify-content: center;
  padding-bottom: 1em;
  font-family: 'DIMISTRI', sans-serif;
  letter-spacing: 1px;
  color: #000000;
  font-size: 2.2em;
}
.contactWeGlobal {
  display: flex;
  justify-content: center;
  background-color: rgb(255, 123, 0);
}
.contactWe1 {
  width: 75%;
  background-color: rgb(255, 255, 255);
  padding: 30px;
  margin: 10px;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  margin-top: 1.3em;
}
.contactWe1 h2 {
  font-size: 24px;
  color: #000000;
  margin-bottom: 10px;
}
.contactWe1 p {
  font-size: 16px;
  color: #000000;
  margin-bottom: 20px;
}

.contactForm {
  display: grid;
  grid-template-columns: 1fr;
  gap: 15px;
}

.formGroup{
  display: flex;
  flex-direction: column;
}
.nameBackg{
  background-color:  rgb(255, 255, 255);
  color: black;
}
.formGroup label{
  font-size: 18px;
  color: #000000;
  margin-bottom: 5px;
}

.formGroup input, .formGroup textarea {
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
  font-size: 16px;
}
::placeholder {
    color: rgb(137, 137, 137);
}
.formGroup textarea {
  resize: vertical;
}
.btnSubmit{
  display: flex;
  justify-content: center;
  align-items: center;
  height: 5em;
}
.btnSubmit1{
  height: 2.8em;
}
button[type="submit"] {
  padding: 10px 20px;
  background-color: #ff7b00;
  color: #fff;
  border: none;
  border-radius: 5px;
  font-size: 16px;
  cursor: pointer;
  transition: background-color 0.3s ease;
  width: 70%;
  box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.5);
}
button[type="submit"]:hover {
  background-color:  rgba(255, 10, 6, 0.883);
  width: 70%;
}
</style>