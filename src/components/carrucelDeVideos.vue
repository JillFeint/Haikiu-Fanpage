<template>
  <div class="galleryGlobalContainer1">
    <section class="seccion01">
        <div class="videoContainer1">
            <div class="wrapper1">
              <div class="wrapper-holder1">
                <video autoplay loop muted id="slider-video-1">
              <source src="../assets/seccion.mp4" type="video/mp4">
                </video>
                <div id="slider-img-1"></div>
                <div id="slider-img-2"></div>
                <div id="slider-img-3"></div>
              </div>
            </div>
            <div class="button-holder1">
              <a href="#slider-video-1" class="button-slider1"></a>
              <a href="#slider-img-1" class="button-slider1"></a>
              <a href="#slider-img-2" class="button-slider1"></a>
              <a href="#slider-img-3" class="button-slider1"></a>
            </div>
        </div> 
      </section>
  </div>
</template>

<script>

</script>


<style>
.seccion01 {
  position: relative;
  width: 100%;
  height: 23em;
  overflow: hidden; 
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: rgb(53, 54, 68);
}
.videoContainer1{
  background-color: rgb(255, 123, 0);
  position: relative;
  height: 100%;
  width: 50%;
}
.videoContainer1 .wrapper1 {
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden;
}
.videoContainer1 .wrapper-holder1 {
  display: grid;
  grid-template-columns: repeat(4, 100%);
  width: 100%;
  height: 100%;
}
.videoContainer1 #slider-video-1 {
  background-position: center;
  background-size: cover;
  width: 100%;
  height: 100%;
}
.videoContainer1 #slider-img-1 {
  background-image: url(../assets/1.jpeg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.videoContainer1 #slider-img-2 {
  background-image: url(../assets/2.jpeg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.videoContainer1 #slider-img-3 {
  background-image: url(../assets/3.jpeg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.button-slider1 {
  background-color: white;
  width: 15px;
  height: 15px;
  border-radius: 15px;
  display: inline-block;
  margin: 5px;
}
.button-slider1:hover {
  background-color: gray;
}
.videoContainer1 .button-holder1 {
  position: absolute;
  left: 45%;
  bottom: 0%;
}
.video-seccion1 {
  width: 50em;
  height: auto;
}
</style>