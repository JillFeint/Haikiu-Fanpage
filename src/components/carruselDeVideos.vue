<template>
  <div class="body-carrucel">
    <div class="container-carrucel">
      <div class="mySlides">
        <img src="../assets/1.jpeg" alt="imagen-1">
      </div>
      <div class="mySlides">
        <img src="../assets/2.jpeg" alt="">
      </div>
      <div class="mySlides">
        <img src="../assets/3.jpeg" alt="">
      </div>
      
      <a class="prev-carrucel" @click="plusSlides(-1)">&#10094;</a>
      <a class="next-carrucel" @click="plusSlides(1)">&#10095;</a>

      <div class="elements-carrucel">
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
.body-carrucel{
  width: 100%;
  max-width: 1450px;
  height: 80%;
  padding: 40px;
  background-color: rgb(255, 123, 0);
  background-attachment: fixed;
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  justify-content: center;
  align-items: center;
}
.container-carrucel{
  width: 50%;
  position: relative;
}
.mySlides{
  display: none;
}
.mySlides img{
  width: 100%;
}
.prev-carrucel, .next-carrucel{
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
.next-carrucel{
  right: 0;
  border-radius: 3px 0 0 3px;
}
.prev-carrucel:hover, .next-carrucel:hover{
  background-color: rgba(0, 0, 0, 0.8);
}
.elements-carrucel{
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
@media screen and (max-width:900px) {
  .container-carrucel{
      width: 100%;
  }
}
@media screen and (max-width:500px) {
  .container-carrucel{
      width: 100%;
  }
  .prev-carrucel, .next-carrucel{
      padding: 5px;
  }
}

</style>