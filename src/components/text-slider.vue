
<template>
    <section class="position-relative">
        <div class="container">
            <div class="row">
                <div class="col-md-5 before">
                    <h2>Lorum ipsum</h2>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam aliquid sapiente maxime illum facilis. Laboriosam excepturi adipisci culpa, magnam aut qui corrupti, saepe repudiandae atque nisi molestias iure alias accusamus!</p>
                </div>
                <div class="offset-md-2 col-md-5">
                    <swiper class="h-100"
                        :slides-per-view="1.5"
                        :space-between="20"
                        :autoplay="{
                            delay: 2500,
                            disableOnInteraction: false,
                            reverseDirection: true,
                        }"
                        :modules="modules"
                        :breakpoints="{
                            767: {
                            slidesPerView: 2
                            }
                        }"
                    >
                        <swiper-slide>  
                            <div class="slide-container">
                                <img class="w-100 h-100" src="../assets/feest-s800x600.jpg" alt="Sunburst Festival">
                                <div class="background"></div>
                                <h3>Sunburst Festival</h3>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="slide-container">
                                <img class="w-100 h-100" src="../assets/istockphoto-1298329918-612x612.jpg" alt="Sunny beach Festival">
                                <h3>Sunny beach Festival</h3>
                                <div class="background"></div>

                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="slide-container">
                                <img class="w-100 h-100" src="../assets/istockphoto-1298329918-612x612.jpg" alt="Sunny beach Festival">
                                <h3>Sunny beach Festival</h3>
                                <div class="background"></div>

                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="slide-container">
                                <img class="w-100 h-100" src="../assets/istockphoto-1298329918-612x612.jpg" alt="Sunny beach Festival">
                                <h3>Sunny beach Festival</h3>
                                <div class="background"></div>

                            </div>
                        </swiper-slide>
                    </swiper>
                </div>
            </div>
        </div>
    </section>
</template>
  
<script>
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/swiper-bundle.css';

import { Autoplay } from 'swiper/modules';

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
        modules: [Autoplay],
    };
  },

};

</script>

<style scoped>
 .swiper {
    cursor: grabbing;
 }

 .slide-container {
    position: relative;
    height: 100%;
    min-height: 250px;
 }
 .slide-container img {
    position: absolute;
    width: 100%;
    height: 100%;
    object-fit: cover;
    z-index: 1;
 }
 .slide-container h3 {
    z-index: 3;
    position: relative;
    padding: .4rem;
    font-size: .7rem;
    width: 50%;
 }

 .slide-container .background {
    background-color: black;
    opacity: .5;
    position: absolute;
    width: 100%;
    height: 100%;
    z-index: 2;
    top: 0;
 }
</style>
  