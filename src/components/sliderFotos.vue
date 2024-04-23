<template>
    <div class="body-sliderFotos">
        <div class="container-sliderFotos">
            <span class="slider-fotos" id="slider1"></span>
            <span class="slider-fotos" id="slider2"></span>
            <span class="slider-fotos" id="slider3"></span>
            <span class="slider-fotos" id="slider4"></span>
            <span class="slider-fotos" id="slider5"></span>
            <span class="slider-fotos" id="slider6"></span>
            <span class="slider-fotos" id="slider7"></span>
            <div class="imgContainer-sliderFotos">
                <div class="slide_div-fotos" id="slide_1">
                    <img src="../assets/1.jpeg" alt="" class="img-sliderFotos" id="img1">
                    <a href="#slider1" class="button-sliderFotos" id="button1"></a>
                </div>
                <div class="slide_div-fotos" id="slide_2">
                    <img src="../assets/2.jpeg" alt="" class="img-sliderFotos" id="img2">
                    <a href="#slider2" class="button-sliderFotos" id="button2"></a>
                </div>
                <div class="slide_div-fotos" id="slide_3">
                    <img src="../assets/3.jpeg" alt="" class="img-sliderFotos" id="img3">
                    <a href="#slider3" class="button-sliderFotos" id="button3"></a>
                </div>
                <div class="slide_div-fotos" id="slide_4">
                    <img src="../assets/4.jpeg" alt="" class="img-sliderFotos" id="img4">
                    <a href="#slider4" class="button-sliderFotos" id="button4"></a>
                </div>
                <div class="slide_div-fotos" id="slide_5">
                    <img src="../assets/5.jpeg" alt="" class="img-sliderFotos" id="img5">
                    <a href="#slider5" class="button-sliderFotos" id="button5"></a>
                </div>
                <div class="slide_div-fotos" id="slide_6">
                    <img src="../assets/6.jpeg" alt="" class="img-sliderFotos" id="img6">
                    <a href="#slider6" class="button-sliderFotos" id="button6"></a>
                </div>
                <div class="slide_div-fotos" id="slide_7">
                    <img src="../assets/7.jpeg" alt="" class="img-sliderFotos" id="img7">
                    <a href="#slider7" class="button-sliderFotos" id="button7"></a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
.body-sliderFotos{
    width: 100%;
    height: 100vh;
    display: flex;
    align-items: center;
    overflow: hidden;
    background: linear-gradient(30deg, rgb(100, 241, 84), rgb(92, 92, 229), rgb(111, 30, 30));
}

.container-sliderFotos{
    width: 100%;
    height: 90vh;
    display: flex;
    flex-direction: row;
    align-items: center;
    overflow: hidden;
}

.imgContainer-sliderFotos{
    width: 100%;
    height: 600px;
    position: absolute;
    left: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    transition: 1s;
}

.slide_div-fotos{
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 30px 0 30px;
}

.img-sliderFotos{
    position: relative;
    height: 370px;
    width: 240px;
    filter: saturate(10%);
    transition: 0.7s;
    background-color: rgba(0, 0, 0, 0.4);
    border-radius: 20px;
}

.button-sliderFotos{
    position: absolute;
    width: 240px;
    height: 370px;
    transition: 0.7s;
    background-color: rgba(0, 0, 0, 0.4);
    border-radius: 20px;
}
.button-sliderFotos:hover{
    background-color: rgba(0, 0, 0, 0.2);
}
#slider1:target ~ .imgContainer-sliderFotos #img1,
#slider1:target ~ .imgContainer-sliderFotos #button1{
    width: 390px;
    height: 600px;
    background-color: transparent;
    filter: saturate(100%);
}
#slider2:target ~ .imgContainer-sliderFotos #img2,
#slider2:target ~ .imgContainer-sliderFotos #button2{
    width: 390px;
    height: 600px;
    background-color: transparent;
    filter: saturate(100%);
}
#slider3:target ~ .imgContainer-sliderFotos #img3,
#slider3:target ~ .imgContainer-sliderFotos #button3{
    width: 390px;
    height: 600px;
    background-color: transparent;
    filter: saturate(100%);
}
#slider4:target ~ .imgContainer-sliderFotos #img4,
#slider4:target ~ .imgContainer-sliderFotos #button4{
    width: 390px;
    height: 600px;
    background-color: transparent;
    filter: saturate(100%);
}
#slider5:target ~ .imgContainer-sliderFotos #img5,
#slider5:target ~ .imgContainer-sliderFotos #button5{
    width: 390px;
    height: 600px;
    background-color: transparent;
    filter: saturate(100%);
}
#slider6:target ~ .imgContainer-sliderFotos #img6,
#slider6:target ~ .imgContainer-sliderFotos #button6{
    width: 390px;
    height: 600px;
    background-color: transparent;
    filter: saturate(100%);
}
#slider7:target ~ .imgContainer-sliderFotos #img7,
#slider7:target ~ .imgContainer-sliderFotos #button7{
    width: 390px;
    height: 600px;
    background-color: transparent;
    filter: saturate(100%);
}
#slider1:target ~ .imgContainer-sliderFotos{
    left: 60%;
}
#slider2:target ~ .imgContainer-sliderFotos{
    left: 40%;
}
#slider3:target ~ .imgContainer-sliderFotos{
    left: 20%;
}
#slider4:target ~ .imgContainer-sliderFotos{
    left: 0%;
}
#slider5:target ~ .imgContainer-sliderFotos{
    left: -20%;
}
#slider6:target ~ .imgContainer-sliderFotos{
    left: -40%;
}
#slider7:target ~ .imgContainer-sliderFotos{
    left: -60%;
}
.img-sliderFotos{
    height: 370px;
}

</style>