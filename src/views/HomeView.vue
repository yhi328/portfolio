<template>
  <div>
    <v-container>
      <div class="section"></div>
      <v-parallax
    dark
    src = "/portfolio/image/head.jpg"
  >
    <v-layout
      align-center
      column
      justify-center
    >  <hr><hr>
    <div class="MainTitle">
      <h1 class="display-2 font-weight-thin mb-3"><TextAnime3 :autoplay="autoplay"/></h1></div>
      <h4 class="subheading"><br>안녕하세요. 남들과는 다른 새로운 것을 추구하는 윤혜인입니다.
    <br>틀에 박힌 사고를 항상 경계하고 새로운 방향으로 나아가려 합니다.
    <br>다양한 아이디어 경진대회 경험으로 신선한 사고를 위해 노력해왔습니다.
    <br>이제는 그 경험을 세상에 펼칠 시간인 거 같습니다.
  </h4>
    <hr><hr>
    </v-layout>
  </v-parallax>
    
    </v-container>

    <v-divider></v-divider>

<v-container>
  <div class="section"></div>
   <v-layout justify-space-around>
    <v-flex xs1>
    <v-img id="sec1" data-aos="zoom-in" src="/portfolio/image/profile.jpg" aspect-ratio="1"></v-img>
    </v-flex>
    </v-layout>
    <br>

  <v-layout
      align-center
      column
      justify-center
    >
   
<TextAnime2 v-if="anime2"/>
<TextAnime1 v-if="anime1"/>
<div id="sec1" data-aos="fade">명지전문대학 정보통신공학과</div>
<div id="sec1" data-aos="fade"> 전공심화 졸업예정</div><br>
</v-layout>
<div class="section"></div>
</v-container>
<v-divider></v-divider>

    <!-- fade, zoom -->
    <div class="section">
      <div id="sec1" data-aos="fade">
        <div class="header">Certificate</div>
      </div>
      </div>
<!-- 자격증 -->
<v-container>
  <v-layout
      align-center
      column
      justify-center
    >
  <v-row>
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
  </v-layout>
  <div class="section"></div>
</v-container>

    <v-divider></v-divider>

          <!-- fade, zoom -->
          <div class="section">
      <div id="sec1" data-aos="fade">
        <div class="header">Skills</div>
      </div>
      </div>
<v-container>
    <!-- 언어 -->
    <v-container fluid>
    <v-layout justify-space-around>
      <v-flex xs5>
        <v-layout row>
          <div class="subheading">Program</div>&nbsp;&nbsp;
          <v-img id="sec1" data-aos="zoom-in-up" src="/portfolio/image/mysql.png" aspect-ratio="1"></v-img>
          <v-img id="sec1" data-aos="zoom-in-up" src="/portfolio/image/python.png" aspect-ratio="1"></v-img>
          <v-img id="sec1" data-aos="zoom-in-up" src="/portfolio/image/vsc.png" aspect-ratio="1"></v-img>
          <v-img id="sec1" data-aos="zoom-in-up" src="/portfolio/image/arduino.png" aspect-ratio="1"></v-img>
          <v-img id="sec1" data-aos="zoom-in-up" src="/portfolio/image/vuejs.png" aspect-ratio="1"></v-img>
        </v-layout>

        <v-layout row>
          <div class="subheading">Design</div>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
          <v-img id="sec1" data-aos="zoom-in-down" src="/portfolio/image/Illustrator.png" aspect-ratio="1"></v-img>
          <v-img id="sec1" data-aos="zoom-in-down" src="/portfolio/image/photoshop.png" aspect-ratio="1"></v-img>
          <v-img id="sec1" data-aos="zoom-in-down" src="/portfolio/image/aftereffects.png" aspect-ratio="1"></v-img>
          <v-img id="sec1" data-aos="zoom-in-down" src="/portfolio/image/premierepro.png" aspect-ratio="1"></v-img>
          <v-img id="sec1" data-aos="zoom-in-down" src="/portfolio/image/cinema.jpg" aspect-ratio="1"></v-img>
        </v-layout>
      </v-flex>
    </v-layout>
    <div class="section"></div>
  </v-container>

</v-container>
    

  <v-divider></v-divider>

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
        color="#e9967a"
        large
      >
        <template v-slot:icon>
          <span><v-icon color=white>mdi-license </v-icon></span>
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
        color="#FFDAB9"
        icon-color="white"
        small
      >
        <v-layout justify-space-between>
          <v-flex xs7>2019년 창업아이디어 경진대회 장려상</v-flex>
          <v-flex xs5 text-xs-right>2019.10.27</v-flex>
        </v-layout>
      </v-timeline-item>

      <v-timeline-item
        class="mb-3"
        color="#FFDAB9"
        icon-color="white"
        small
      >
        <v-layout justify-space-between>
          <v-flex xs7>
            2020년 캠퍼스 CEO 육성사업 스타트업 아이디어 경진대회 우수상
          </v-flex>
          <v-flex xs5 text-xs-right>2020.06.19</v-flex>
        </v-layout>
      </v-timeline-item>

      <v-timeline-item
        class="mb-3"
        color="#FFDAB9"
        icon-color="white"
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
        color="#FFDAB9"
        icon-color="white"
        small
      >
        <v-layout justify-space-between>
          <v-flex xs7>
            <v-chip
              class="white--text ml-0"
              color="#FFA500"
              label
              small
            >
              Special
            </v-chip>
            2020 여성발명왕 EXPO 동국대상
          </v-flex>
          <v-flex xs5 text-xs-right>2020.10.25</v-flex>
        </v-layout>
      </v-timeline-item>

      <v-timeline-item
        class="mb-3"
        color="#FFDAB9"
        icon-color="white"
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
        class="mb-3"
        color="#FFDAB9"
        icon-color="white"
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
        class="mb-3"
        color="#FFDAB9"
        icon-color="white"
        small
      >
        <v-layout justify-space-between>
          <v-flex xs7>
            <v-chip
              class="white--text ml-0"
              color="#FFA500"
              label
              small
            >
              1st
            </v-chip>
            2021년 명지전문대학 정보통신공학과 학술제 금상 
          </v-flex>
          <v-flex xs5 text-xs-right>2021.12.17</v-flex>
        </v-layout>
      </v-timeline-item>
      <v-timeline-item
        class="mb-3"
        color="#FFDAB9"
        icon-color="white"
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
    <div class="section"></div>
  </v-container>

  <v-divider></v-divider>

  <div id="foo" v-on:click="select($event)"></div>
    <!-- fade, zoom -->
    <div class="section">
      <div id="sec1" data-aos="fade">
        <div class="header">Projects</div>
      </div>
      </div>
    <v-container>
    <!-- 프로젝트 -->
    <v-layout>
    
      <v-card>
<swiper :options="swiperOption" class="swiper">
      <swiper-slide data-aos="fade-in" data-aos-duration="1000" class="slide" style="background-image:url(/portfolio/image/project1_b.jpg);">
       <v-layout data-aos="fade-up" data-aos-duration="1000" fill-height align-center justify-center>
        <div class="slog">Pet Food Checking Program</div>
       </v-layout>
      </swiper-slide>
      <swiper-slide class="slide" style="background-image:url(/portfolio/image/project2_b.jpg);">
        <v-layout fill-height align-center justify-center>
        <div class="slog">방문자 발열체크 및 안심번호 팔찌 인식을 통한 개인정보 관리 시스템</div>
       </v-layout>
      </swiper-slide>
      <swiper-slide class="slide" style="background-image:url(/portfolio/image/project3_b.jpg);">
        <v-layout fill-height align-center justify-center>
        <div class="slog">Kakao Oven을 활용한 웹페이지 제작</div>
       </v-layout>
      </swiper-slide>
    </swiper>
  <v-card-title primary-title align-center>
          <div>
            <h3 class="headline mb-0">옆으로 넘겨보세요</h3>
            <div align-center> {{ card_text }} </div>
          </div>
        </v-card-title>
      </v-card>

  </v-layout>
  <div class="section"></div>
</v-container>

<v-divider></v-divider>

<!-- 푸터 -->
<v-container>
<v-parallax
    dark
    src = "/portfolio/image/footer.jpg"
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
</v-container>
  
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from 'vue-awesome-swiper'
import 'swiper/swiper-bundle.css'
import AOS from "aos"
import "aos/dist/aos.css";

import TextAnime1 from './TextAnime1'
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
        anime1: true,
        anime2: true,
      autoplay: true,
      }
    },
    mounted(){
      AOS.init()
    },  
    components:{
      Swiper,
      SwiperSlide,

      TextAnime1,
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
        font-size:40px;
        font-weight:bold;
        color:black;
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
  background:	#eebfac;
  font-size: initial;
}

.card__face--back {
  background: #BC8F8F;
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
    font-weight: light;
  }

  .headline {
    font-size:30px;
    font-weight:thin;
    text-align: center;
    box-align: center;
  }
</style>