<template>
  <div class="body-carrusel">
    <div class="container-carrusel">
      <div class="mySlides">
        <div class="image-container">
        <img src="../assets/HD/hd-1.jpg" alt="imagen-1">
      </div>
      </div>
      <div class="mySlides">
        <div class="image-container">
        <img src="../assets/HD/hd-2.jpg" alt="">
      </div>
      </div>
      <div class="mySlides">
        <div class="image-container">
        <img src="../assets/HD/hd-3.jpg" alt="">
      </div>
      </div>
      <div class="flechas-carrusel">
        <a class="prev-carrusel" @click="plusSlides(-1)">&#10094;</a>
        <a class="next-carrusel" @click="plusSlides(1)">&#10095;</a>
      </div>
      <div class="elements-carrusel">
        <span class="quadrate" @click="currentSlide(1)"></span>
        <span class="quadrate" @click="currentSlide(2)"></span>
        <span class="quadrate" @click="currentSlide(3)"></span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      slideIndex: 1,
    };
  },
  mounted() {
    this.showSlides(this.slideIndex);
  },
  methods: {
    plusSlides(n) {
      this.showSlides(this.slideIndex += n);
    },
    currentSlide(n) {
      this.showSlides(this.slideIndex = n);
    },
    showSlides(n) {
      const slides = document.querySelectorAll(".mySlides");
      const quadrates = document.querySelectorAll(".quadrate"); 
      if (n > slides.length) this.slideIndex = 1;
      if (n < 1) this.slideIndex = slides.length;
      slides.forEach(slide => {
        slide.style.display = "none";
      });
      quadrates.forEach(quadrate => {
        quadrate.classList.remove("active");
      });
      slides[this.slideIndex - 1].style.display = "block";
      quadrates[this.slideIndex - 1].classList.add("active");
    }
  }
};
</script>

<style>
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
.body-carrusel{
  width: 100%;
  height: 100%;
  padding: 50px;
  background-color: rgb(53, 54, 68);
  display: flex;
  justify-content: center;
  align-items: center;
}
.container-carrusel{
  width: 100%;
  height: 100%;
  position: relative;
}
.mySlides{
  display: none;
}
.image-container {
  width: 100%;
  height: 100%;
  /* padding-bottom: 75%; */
  position: absolute;
}
.image-container img {
  position: relative;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
.prev-carrusel, .next-carrusel{
  cursor: pointer;
  position: absolute;
  top: 50%;
  width: auto;
  margin-top: -22px;
  padding: 16px;
  color: #fff;
  font-weight: bold;
  font-size: 18px;
  transition: 0.6 ease;
  border-radius: 0 3px 3px 0;
  user-select: none;
  border:  solid #fff 2px;
}
.next-carrusel{
  right: 0;
  border-radius: 3px 0 0 3px;
}
.prev-carrusel:hover, .next-carrusel:hover{
  background-color: rgba(0, 0, 0, 0.8);
}
.elements-carrusel{
  text-align: center;
}
.quadrate{
  cursor: pointer;
  height: 4px;
  width: 50px;
  margin: 0 2px;
  background-color: #717171;
  display: inline-block;
  transition: background-color 0.6s ease;
  border-radius: 2px;
}
.active, .quadrate:hover{
  background-color: #fff;
}
@media screen and (min-width: 767px) and (max-width: 1025px){
  .body-carrusel{
  width: 100%;
  height: 100%;
  padding: 0 30%; 
  background-color: rgb(53, 54, 68);
  display: flex;

 } 
  .container-carrusel{
  width: 70%;
  }
  .image-container {
  height: 100%;
  position: absolute;
  display: flex;
  justify-content: center;
  padding: 20px 0;
  }
  .image-container img {
  position: relative;
  max-height: 100%;
  max-width: 100%;
  width: auto;
}
}
@media screen and (min-width: 100px) and (max-width: 767px){
  .container-carrusel{
      width: 80%;
  }
  .prev-carrusel, .next-carrusel{
      padding: 5px;
  }
}

</style>