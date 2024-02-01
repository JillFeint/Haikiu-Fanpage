<template>
  <div class="contactWeGlobal">
  <div class="contactWe1">
    <h2>Contactanos</h2>
    <p>Por favor, envíanos tus consultas y comentarios. Estaremos encantados de ayudarte.</p>
    <form class="contactForm">
      <div class="formGroup">
        <label for="name">Nombre:</label>
        <input type="text" id="name" name="name" placeholder="Ingresa tu nombre">
      </div>
      <div class="formGroup">
        <label for="email">Correo electrónico:</label>
        <input type="email" id="email" name="email" placeholder="Ingresa tu correo electrónico">
      </div>
      <div class="formGroup">
        <label for="message">Mensaje:</label>
        <textarea id="message" name="message" rows="4" placeholder="Escribe aquí tu mensaje"></textarea>
      </div>
      <button type="submit">Enviar mensaje</button>
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

.contactWeGlobal {
display: flex;
justify-content: center;
background-color: #ff9900;
}
.contactWe1 {
  width: 80%;
  background-color: azure;
  padding: 30px;
  margin: 10px;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.contactWe h2 {
  font-size: 24px;
  color: #333;
  margin-bottom: 10px;
}

.contactWe p {
  font-size: 16px;
  color: #666;
  margin-bottom: 20px;
}

.contactForm {
  display: grid;
  grid-template-columns: 1fr;
  gap: 15px;
}

.formGroup {
  display: flex;
  flex-direction: column;
}

.formGroup label {
  font-size: 16px;
  color: #333;
  margin-bottom: 5px;
}

.formGroup input, .formGroup textarea {
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
  font-size: 16px;
}

.formGroup textarea {
  resize: vertical;
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
}

button[type="submit"]:hover {
  background-color: #ff6300;
}
</style>