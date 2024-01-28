<template>
  <div>
    <header class="header"> 
    </header>
    <nav class="nav">
      <div class="div-header">
        <ul class="ul-nav">
          <li class="btn-header border-li1"><a href="#">Inicio</a></li>
          <li class="btn-header"><a href="#">Contactanos</a></li>
          <li class="btn-header"><a href="#">Equipo</a></li>
          <li class="btn-header"><a href="#">Partidos</a></li>
          <li class="btn-header border-li2"><a href="#">Informacion</a></li>
        </ul>
      </div>
      </nav>
      <section class="seccion1">
        <video autoplay loop muted class="video-seccion">
          <source src="./assets/seccion.mp4" type="video/mp4">
        </video>
        </section>
      <section class="seccion2">
        <div class="div1-seccion2">
          <h2>Quienes Somos</h2>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tenetur minima voluptatum nisi earum sapiente
          deserunt. Repellendus repudiandae nostrum, non quas facere perferendis rerum eos adipisci harum minus porro natus vitae?</p>
        </div>
        <div class="div2-seccion2">
          <h2>Reglas</h2>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dicta ex aliquam temporibus dolore quam consequuntur
            itaque porro sapiente minus voluptate illum quaerat architecto voluptatem assumenda quisquam nesciunt, facilis cum consequatur!</p>
          </div>
          <div class="div3-seccion2">
            <div class="div-logo">
              <img class="logo" src="./assets/logo.png" alt="">
          </div>
          </div>
          <div class="div4-seccion2">
            <form class="form-seccion2" action="">
              <input class="input-seccion2" type="checkbox"><label for="">primero</label>
              <input class="input-seccion2" type="checkbox"><label for="">segundo</label>
              <input class="input-seccion2" type="checkbox"><label for="">tercero</label>
              <input class="input-seccion2" type="checkbox"><label for="">cuarto</label>
              <button type="sumit">aceptar</button>
            </form>
          </div>
        </section>
        <section class="seccion3">
          <div class="div-seccion3">
          <h2>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore adipisci rerum, molestiae quae recusandae ab incidunt tenetur vero asperiores quisquam facilis, perferendis nostrum! Voluptatum earum ducimus aliquam, reprehenderit delectus cumque?
          </h2>
          <p> pLorem ipsum dolor sit amet.
          pLorem ipsum dolor sit amet consectetur adipisicing elit. Necessitatibus perferendis ullam fugit sint natus quis quaerat! Dolorum, debitis. Soluta totam molestias, dolorem neque unde esse nisi quod facilis laudantium quibusdam!
          pLorem ipsum dolor sit amet consectetur adipisicing elit. Necessitatibus perferendis ullam fugit sint natus quis quaerat! Dolorum, debitis. Soluta totam molestias, dolorem neque unde esse nisi quod facilis laudantium quibusdam!
          pLorem ipsum dolor sit amet consectetur adipisicing elit. Necessitatibus perferendis ullam fugit sint natus quis quaerat! Dolorum, debitis. Soluta totam molestias, dolorem neque unde esse nisi quod facilis laudantium quibusdam!
          pLorem ipsum dolor sit amet consectetur adipisicing elit. Necessitatibus perferendis ullam fugit sint natus quis quaerat! Dolorum, debitis. Soluta totam molestias, dolorem neque unde esse nisi quod facilis laudantium quibusdam!4</p>
        </div>
        </section>
        <section class="seccion4">
          <p> pLorem ipsum dolor sit amet.
          pLorem ipsum dolor sit amet consectetur adipisicing elit. Necessitatibus perferendis ullam fugit sint natus quis quaerat! Dolorum, debitis. Soluta totam molestias, dolorem neque unde esse nisi quod facilis laudantium quibusdam!
          pLorem ipsum dolor sit amet consectetur adipisicing elit. Necessitatibus perferendis ullam fugit sint natus quis quaerat! Dolorum, debitis. Soluta totam molestias, dolorem neque unde esse nisi quod facilis laudantium quibusdam!
          pLorem ipsum dolor sit amet consectetur adipisicing elit. Necessitatibus perferendis ullam fugit sint natus quis quaerat! Dolorum, debitis. Soluta totam molestias, dolorem neque unde esse nisi quod facilis laudantium quibusdam!
          pLorem ipsum dolor sit amet consectetur adipisicing elit. Necessitatibus perferendis ullam fugit sint natus quis quaerat! Dolorum, debitis. Soluta totam molestias, dolorem neque unde esse nisi quod facilis laudantium quibusdam!4</p>
        </section>
        <footer>
          <p>angel gay y mandon</p>
        </footer>
  </div>
</template>

<script>
export default {

}
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
.header {
  width: 100%;
  height: 32vh;
  display: flex;
  background-image: url("./assets/header.png");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center center;
  margin: 0;
  padding: 0; 
  box-sizing: border-box; 
  justify-content: center;
}
.div-logo {
  display: flex;
  justify-content: center;
  align-items: center;
}
.logo {
  width: 180px;
  height: 200px;
}
.nav {
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: black ;

}
.ul-nav {
  list-style: none;
  display: flex;
}
.btn-header a {
  text-decoration: none;
  background-color: orangered;
  color: rgb(255, 255, 255);
  padding: 10px;
  font-size: 20px;
  padding-left: 10px;
  padding-right: 10px;
}
.border-li1 a {
  border-top-left-radius: 10px;
}
.border-li2 a {
  border-top-right-radius: 10px;
}
.btn-header a:hover{
  background-color: rgb(177, 70, 31);
  color: white;
  padding: 10px;
  border-radius: 5px;
}
.seccion1 {
  position: relative;
  width: 100%;
  height: 400px;
}

.video-seccion {
  width: 100%;
  height: 100%;
  object-fit: cover;;
} 
.seccion2 {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: 1fr 1fr;
}
h2 {
  padding: 5px;
}
.div1-seccion2 {
  grid-row: 1;
  grid-column: 1;
  background-color: aquamarine;
  padding: 10px;
  height: 10rem;
}
.div2-seccion2 {
  grid-row: 2;
  grid-column: 1;
  background-color: blanchedalmond;
  padding: 10px;
  height: 10rem;
}
.div3-seccion2 {
  grid-row: 1;
  grid-column: 2;
  background-color: blueviolet;
  padding: 10px;
  height: 10rem;
}
.div4-seccion2 {
  grid-row: 2;
  grid-column: 2;
  background-color: blue;
  padding: 10px;
  height: 10rem;
}
.form-seccion2 {
  display: flex;
  flex-direction: column;
}
.seccion3 {
  height: 100%;
  width: 100%;
  background-color: black;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: justify;
  color: white;
}
.div-seccion3 {
  height: 70%;
  width: 70%;
  background-color: rgb(255, 255, 255);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: justify;
  color: rgb(0, 0, 0);
}
.seccion4 {
  height: 100%;
  width: 100%;
  background-color: rgb(255, 0, 0);
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: justify;
  color: white;
  padding: 15px;
}
</style>
