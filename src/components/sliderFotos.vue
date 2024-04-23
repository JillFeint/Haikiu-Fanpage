<template>
    <div class="body-sliderFotos">
        <div class="container-sliderFotos" ref="container">
            <div class="imgContainer-sliderFotos" ref="imgContainer">
                <div class="slide_div-fotos">
                    <img src="../assets/1.jpeg" alt="" class="img-sliderFotos" :id="'img1'" @click="activateImage(1)">
                </div>
                <div class="slide_div-fotos">
                    <img src="../assets/2.jpeg" alt="" class="img-sliderFotos" :id="'img2'" @click="activateImage(2)">
                </div>
                <div class="slide_div-fotos">
                    <img src="../assets/3.jpeg" alt="" class="img-sliderFotos" :id="'img3'" @click="activateImage(3)">
                </div>
                <div class="slide_div-fotos">
                    <img src="../assets/4.jpeg" alt="" class="img-sliderFotos" :id="'img4'" @click="activateImage(4)">
                </div>
                <div class="slide_div-fotos">
                    <img src="../assets/5.jpeg" alt="" class="img-sliderFotos" :id="'img5'" @click="activateImage(5)">
                </div>
                <div class="slide_div-fotos">
                    <img src="../assets/6.jpeg" alt="" class="img-sliderFotos" :id="'img6'" @click="activateImage(6)">
                </div>
                <div class="slide_div-fotos">
                    <img src="../assets/7.jpeg" alt="" class="img-sliderFotos" :id="'img7'" @click="activateImage(7)">
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    methods: {
        activateImage(index) {
            
            const images = document.querySelectorAll('.img-sliderFotos');
            images.forEach(img => img.classList.remove('active'));

            const selectedImg = document.getElementById('img' + index);
            selectedImg.classList.add('active');

            const imgContainer = this.$refs.imgContainer;
            const selectedImgRect = selectedImg.getBoundingClientRect();
            const imgContainerRect = imgContainer.getBoundingClientRect();
            imgContainer.scrollBy({
                top: selectedImgRect.top - imgContainerRect.top - (imgContainerRect.height / 2) + (selectedImgRect.height / 2),
                left: selectedImgRect.left - imgContainerRect.left - (imgContainerRect.width / 2) + (selectedImgRect.width / 2),
                behavior: 'smooth'
            });
        }
    }
}
</script>

<style>
.body-sliderFotos {
    width: 100%;
    height: 100vh;
    display: flex;
    align-items: center;
    overflow: hidden;
    background: linear-gradient(30deg, rgb(100, 241, 84), rgb(92, 92, 229), rgb(111, 30, 30));
}

.container-sliderFotos {
    width: 100%;
    height: 90vh;
    display: flex;
    flex-direction: row;
    align-items: center;
    overflow: hidden;
}

.imgContainer-sliderFotos {
    width: 100%;
    height: 600px;
    position: relative;
    display: flex;
    justify-content: space-between; /* Separación entre las imágenes */
    align-items: center;
    overflow: hidden;
    scroll-behavior: smooth;
}

.slide_div-fotos {
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0 20px; /* Espacio entre las imágenes */
    transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
}

.img-sliderFotos {
    height: 370px;
    width: 240px;
    filter: saturate(10%);
    background-color: rgba(0, 0, 0, 0.4);
    border-radius: 20px;
    cursor: pointer;
    transition: transform 0.3s ease-in-out, box-shadow 0.3s ease-in-out;
}

.img-sliderFotos.active {
    filter: saturate(100%);
    transform: scale(1.1);
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
}
</style>
