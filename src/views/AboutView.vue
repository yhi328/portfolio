<template>
    <div>
        <swiper :options="swiperOption" class="swiper">
      <swiper-slide data-aos="fade-in" data-aos-duration="1000" class="slide" style="background-image:url(image/top1.jpg);">
       <v-layout data-aos="fade-up" data-aos-duration="1000" fill-height align-center justify-center>
        <div class="slog">윤혜인</div>
       </v-layout>
      </swiper-slide>
      <swiper-slide class="slide" style="background-image:url(image/top2.jpg);">
        <v-layout fill-height align-center justify-center>
        <div class="slog">준비된 인재</div>
       </v-layout>
      </swiper-slide>
      <swiper-slide class="slide" style="background-image:url(image/top3.jpg);">
        <v-layout fill-height align-center justify-center>
        <div class="slog">아자아자^._.^</div>
       </v-layout>
      </swiper-slide>
    </swiper>
</div>
</template>



<script>
import { Swiper, SwiperSlide } from 'vue-awesome-swiper'
import 'swiper/swiper-bundle.css'
import AOS from "aos"
import "aos/dist/aos.css";
  export default {
    name: 'AboutView',
    data(){
      return {
        swiperOption:{
          loop:true,
          autoplay:{
            delay:1000
          }
        }
      }
    },
    mounted(){
      AOS.init()
    },  
    components:{
      Swiper,
      SwiperSlide
    }
    
  }
</script>
<style scoped lang="less">
  .swiper{
    height:100vh;
    .slide{
      background-size:cover;
      background-position: center center;
      .slog{
        font-size:60px;
        font-weight:bold;
        color:white;
      }
    }
  }
  .section{
    width:1190px;
    margin: 0 auto;
    padding-top:40px;
    padding-bottom:40px;
    .header{
      text-align:center;
      font-size:40px;
      font-weight:bold;
    }
    .image{
      width:100%;
      height:100%;
      object-fit: cover;
    }
  }
  
</style>