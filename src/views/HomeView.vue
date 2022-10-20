<template>
  <div>
    <v-container>
      <hr><hr>
      <div class="MainTitle">
      <v-container>
      <v-row>
      <TextAnime3 :autoplay="autoplay"/> <div>개발자</div></v-row></v-container></div>
    <br>안녕하세요. 남들과는 다른 새로운 것을 추구하는 예비 개발자 윤혜인입니다.
    <br>틀에 박힌 사고를 항상 경계하고 새로운 방향으로 나아가려 합니다.
    <br>다양한 아이디어 경진대회 경험으로 신선한 사고를 위해 노력해왔습니다.
    <hr><hr>
    </v-container>

    <!--
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
-->

<TextAnime2 v-if="anime2"/>

<!-- 자격증 -->
<v-container>
  <v-row>
<div>
  <p>Certificate</p></div>
    <div class="scene scene--card" data-aos="fade-right">
      <div
        class="card"
        @click="cardOne == 'start' ? (cardOne = 'flipped' ) : (cardOne = 'start' )"
        v-bind:class="{ flipme: cardOne == 'flipped' }"
      >
        <div class="card__face card__face--front">정보처리산업기사</div>
        <div class="card__face card__face--back">2021.11.26</div>
      </div>
    </div>
    <div class="scene scene--card" data-aos="fade-up">
      <div
        class="card"
        @click="cardOne == 'start' ? (cardOne = 'flipped' ) : (cardOne = 'start' )"
        v-bind:class="{ flipme: cardOne == 'flipped' }"
      >
        <div class="card__face card__face--front">파이썬프로그래밍활용능력 2급</div>
        <div class="card__face card__face--back">2021.10.18</div>
      </div>
    </div>
    <div class="scene scene--card" data-aos="fade-down">
      <div
        class="card"
        @click="cardOne == 'start' ? (cardOne = 'flipped' ) : (cardOne = 'start' )"
        v-bind:class="{ flipme: cardOne == 'flipped' }"
      >
        <div class="card__face card__face--front">GTQ그래픽기술자격 1급</div>
        <div class="card__face card__face--back">2022.04.15</div>
      </div>
    </div>
    <div class="scene scene--card" data-aos="fade-left">
      <div
        class="card" 
        @click="cardOne == 'start' ? (cardOne = 'flipped' ) : (cardOne = 'start' )"
        v-bind:class="{ flipme: cardOne == 'flipped' }"
      >
        <div class="card__face card__face--front">컴퓨터그래픽스운용기능사</div>
        <div class="card__face card__face--back">2022.9.16</div>
      </div>
    </div>
  </v-row>
</v-container>

    <v-divider></v-divider>

    <!-- 스크롤위치 -->
    <div id="foo" v-on:click="select($event)"></div>
    <!-- fade, zoom -->
    <div class="section">
      <div id="sec1" data-aos="fade">
        <div class="header">Awards</div>
      </div>
      <!--
      <div class="header">프로젝트 목록</div>-->

      <!--
      <v-layout wrap>
       
        <v-flex xs4 class="pa-2" data-aos="fade-right">
          <v-responsive :aspect-ratio="1/1">
            <img src="/portfolio/image/top1.jpg" class="image">
          </v-responsive>
        </v-flex>
        <v-flex xs4 class="pa-2" data-aos="fade-down" data-aos-delay="100">
          <v-responsive :aspect-ratio="1/1">
            <img src="image/top2.jpg" class="image">
          </v-responsive>
        </v-flex>
        <v-flex xs4 class="pa-2" data-aos="fade-left" data-aos-delay="200">
          <v-responsive :aspect-ratio="1/1">
            <img src="image/top3.jpg" class="image">
          </v-responsive>
        </v-flex>
        <v-flex xs4 class="pa-2" data-aos="fade-right">
          <v-responsive :aspect-ratio="1/1">
            <img src="image/top2.jpg" class="image">
          </v-responsive>
        </v-flex>
        <v-flex xs4 class="pa-2">
          <v-responsive :aspect-ratio="1/1" data-aos="fade-up"  data-aos-delay="100">
            <img src="image/top3.jpg" class="image">
          </v-responsive>
        </v-flex>
        <v-flex xs4 class="pa-2">
          <v-responsive :aspect-ratio="1/1" data-aos="fade-left" data-aos-delay="200">
            <img src="image/top1.jpg" class="image">
          </v-responsive>
        </v-flex>
      </v-layout>
      -->
    </div>

    <v-divider></v-divider>

    <!-- 언어 -->
    <v-card
    class="elevation-16 mx-auto"
    width="100"
    height="100"
  >
    <v-card-title
      class="headline"
      primary-title
    >
      파이썬
    </v-card-title>
    <v-card-text>
      Python
      <div class="text-xs-center mt-5">
        <v-rating
          v-model="rating"
          color="yellow darken-3"
          background-color="grey darken-1"
          empty-icon="$vuetify.icons.ratingFull"
          half-increments
          hover
        ></v-rating>
      </div>
    </v-card-text>

    <v-divider></v-divider>
  
  </v-card>

  <v-divider></v-divider>

  <!-- 스크롤위치 -->
  <div id="foo" v-on:click="select($event)"></div>
    <!-- fade, zoom -->
    <div class="section">
      <div id="sec1" data-aos="fade">
        <div class="header">Awards</div>
      </div>
      </div>
    <!-- 수상내역 timeline -->
    <v-container style="max-width: 600px;">
    <v-timeline dense clipped>
      <v-timeline-item
        fill-dot
        class="white--text mb-5"
        color="orange"
        large
      >
        <template v-slot:icon>
          <span>Awards</span>
        </template>
        </v-timeline-item>
      <v-slide-x-transition
        group
      >
        <v-timeline-item
          v-for="event in timeline"
          :key="event.id"
          class="mb-3"
          color="pink"
          small
        >
          <v-layout justify-space-between>
            <v-flex xs7 v-text="event.text"></v-flex>
            <v-flex xs5 text-xs-right v-text="event.time"></v-flex>
          </v-layout>
        </v-timeline-item>
      </v-slide-x-transition>

      <v-timeline-item
        class="mb-3"
        color="grey"
        icon-color="black"
        small
      >
        <v-layout justify-space-between>
          <v-flex xs7>2019년 창업아이디어 경진대회 장려상</v-flex>
          <v-flex xs5 text-xs-right>2019.10.27</v-flex>
        </v-layout>
      </v-timeline-item>

      <v-timeline-item
        class="mb-3"
        small
      >
        <v-layout justify-space-between>
          <v-flex xs7>
            <v-chip
              class="white--text ml-0"
              color="purple"
              label
              small
            >
              Special
            </v-chip>
            2020년 캠퍼스 CEO 육성사업 스타트업 아이디어 경진대회 우수상
          </v-flex>
          <v-flex xs5 text-xs-right>2020.06.19</v-flex>
        </v-layout>
      </v-timeline-item>

      <v-timeline-item
        class="mb-3"
        color="grey"
        small
      >
        <v-layout justify-space-between>
          <v-flex xs7>
            공학기술교육혁신선도센터 주관 
산학협력 공동교육캠프 창업아이디어 경진대회 은상
          </v-flex>
          <v-flex xs5 text-xs-right>2020.07.21</v-flex>
        </v-layout>
      </v-timeline-item>

      <v-timeline-item
        class="mb-3"
        color="grey"
        small
      >
        <v-layout justify-space-between>
          <v-flex xs7>
            2020 여성발명왕 EXPO 동국대상
          </v-flex>
          <v-flex xs5 text-xs-right>2020.10.25</v-flex>
        </v-layout>
      </v-timeline-item>

      <v-timeline-item
        color="grey"
        small
      >
        <v-layout justify-space-between>
          <v-flex xs7>
            2020 여성발명왕 EXPO 금상 
          </v-flex>
          <v-flex xs5 text-xs-right>2020.10.29</v-flex>
        </v-layout>
      </v-timeline-item>
      <v-timeline-item
        color="grey"
        small
      >
        <v-layout justify-space-between>
          <v-flex xs7>
            2020년 명지전문대학 창업아이디어 경진대회 동상
          </v-flex>
          <v-flex xs5 text-xs-right>2020.12.28</v-flex>
        </v-layout>
      </v-timeline-item>
      <v-timeline-item
        color="grey"
        small
      >
        <v-layout justify-space-between>
          <v-flex xs7>
            2021년 명지전문대학 정보통신공학과 학술제 금상 
          </v-flex>
          <v-flex xs5 text-xs-right>2021.12.17</v-flex>
        </v-layout>
      </v-timeline-item>
      <v-timeline-item
        color="grey"
        small
      >
        <v-layout justify-space-between>
          <v-flex xs7>
            2021년 명지전문대학 캡스톤디자인 경진대회 장려상
          </v-flex>
          <v-flex xs5 text-xs-right>2021.12.23</v-flex>
        </v-layout>
      </v-timeline-item>
    </v-timeline>
  </v-container>

  <v-divider></v-divider>

    <v-container>
    <!-- 슬라이드 -->
    <v-carousel>
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>
</v-container>

<v-divider></v-divider>

<!-- 푸터 -->
<v-parallax
    dark
    src = "image/footer.jpg"
  >
    <v-layout
      align-center
      column
      justify-center
    >
      <h1 class="display-2 font-weight-thin mb-3">Contact</h1>
      <h4 class="subheading">  <v-icon>mdi-email-outline </v-icon> yunhii328@gmail.com</h4>
    </v-layout>
  </v-parallax>
  
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from 'vue-awesome-swiper'
import 'swiper/swiper-bundle.css'
import AOS from "aos"
import "aos/dist/aos.css";

import TextAnime2 from './TextAnime2'
import TextAnime3 from './TextAnime3'

  export default {
    name: 'Home',
    data(){
      return {
        swiperOption:{
          loop:true,
          autoplay:{
            delay:1000
          }
        },
        cardOne: "start",

        data: () => ({
      rating: 3
    }),
  

    //스크롤
    method: {

    handleScroll(e){
      this.scrollPosition = e.target.scrollTop;

    if(this.scrollPosition > 100){
      console.log("UP")
  } else {
    console.log("DOWN")
  }
}
},

      // 텍스트 애니메이션
        anime2: true,
      autoplay: true,

        //슬라이드
        items: [
          {
            src: "image/top2.jpg"
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg'
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg'
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg'
          }
        ],
      }
    },
    mounted(){
      AOS.init()
    },  
    components:{
      Swiper,
      SwiperSlide,

      TextAnime2,
      TextAnime3,
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
  
  // 자격증 카드
  body {
  font-family: sans-serif;
}

.scene {
  width: 200px;
  height: 260px;
  border: 1px solid #ccc;
  margin: 40px 0;
  perspective: 600px;
}


.card {
  width: 100%;
  height: 100%;
  transition: transform 1s;
  transform-style: preserve-3d;
  cursor: pointer;
  position: relative;
}

.card__face {
  position: absolute;
  width: 100%;
  height: 100%;
  line-height: 260px;
  color: white;
  text-align: center;
  font-weight: bold;
  font-size: 40px;
  backface-visibility: hidden;
}

.card__face--front {
  background:		#FFDAB9;
  font-size: initial;
}

.card__face--back {
  background: 	#FFA07A;
  transform: rotateY(180deg);
  font-size: initial;
}

/* this style is applied when the card is clicked */
.flipme {
  transform: rotateY(180deg);
}
  .MainTitle {
    display: inline-block;
    min-width: 0.3em;
    font-size: 2rem;
    animation: text-in .8s cubic-bezier(0.22, 0.15, 0.25, 1.43) 0s backwards;
  }
</style>