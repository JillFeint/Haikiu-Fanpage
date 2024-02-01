<template>
  <div class="galleryGlobalContainer">
    <section class="seccion1">
        <div class="videoContainer">
            <div class="wrapper">
              <div class="wrapper-holder">
                <video autoplay loop muted id="slider-video-1">
              <source src="../assets/seccion.mp4" type="video/mp4">
                </video>
                <div id="slider-img-1"></div>
                <div id="slider-img-2"></div>
                <div id="slider-img-3"></div>
              </div>
            </div>
            <div class="button-holder">
              <a href="#slider-video-1" class="button-slider"></a>
              <a href="#slider-img-1" class="button-slider"></a>
              <a href="#slider-img-2" class="button-slider"></a>
              <a href="#slider-img-3" class="button-slider"></a>
            </div>
        </div> 
      </section>
  </div>
</template>

<script>

</script>


<style>
.seccion1 {
  position: relative;
  width: 100%;
  height: 23em;
  overflow: hidden; 
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: rgb(255, 166, 0);
}
.videoContainer{
  background-color: rgb(255, 123, 0);
  position: relative;
  height: 100%;
  width: 50%;
}
.videoContainer .wrapper {
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden;
}
.videoContainer .wrapper-holder {
  display: grid;
  grid-template-columns: repeat(4, 100%);
  width: 100%;
  height: 100%;
}
.videoContainer #slider-video-1 {
  background-position: center;
  background-size: cover;
  width: 100%;
  height: 100%;
}
.videoContainer #slider-img-1 {
  background-image: url(../assets/1.jpeg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.videoContainer #slider-img-2 {
  background-image: url(../assets/2.jpeg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.videoContainer #slider-img-3 {
  background-image: url(../assets/3.jpeg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.button-slider {
  background-color: white;
  width: 15px;
  height: 15px;
  border-radius: 15px;
  display: inline-block;
}
.videoContainer .button-holder {
  position: absolute;
  left: 45%;
  bottom: 0%;
}
.video-seccion {
  width: 50em;
  height: auto;
}
</style>