<template>
    <div class="TextAnime1">
      <transition-group tag="div" class="title">
        <span v-for="el in text" :key="el.id" class="item" v-text="el.text"></span>
      </transition-group>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      autoplay: Boolean
    },
    data() {
      return {
        timer: null,
        index: 0,
        // 원본 메시지
        original: [
          '"참신한"',
          '"신선한"',
          '"새로운"'
        ],
        // 분해한 메시지
        messages: [],
        text: ''
      }
    },
    computed: {
      editor: {
        get() { return this.text.map(e => e.text).join('') },
        set(text) { this.text = this.convText(text) }
      }
    },
    watch: {
      autoplay(val) {
        clearTimeout(this.timer)
        if (val) {
          this.ticker()
        }
      }
    },
    methods: {
      // 데모 전용 타이머
      ticker() {
        this.timer = setTimeout(() => {
          if (this.autoplay) {
            this.index = this.index < this.messages.length-1 ? this.index + 1 : 0
            this.text = this.messages[this.index]
            this.ticker()
          }
        }, 5000)
      },
      // 텍스트를 분리해서 객체로 리턴하기
      convText(text) {
        const alms = {}
        const result = text.split('').map(el => {
          alms[el] = alms[el] ? ++alms[el] : 1
          return { id: `${el}_${alms[el]}`, text: el }
        })
        return Object.freeze(result) // 감시하지 않음
      }
    },
    created() {
      this.messages = this.original.map(el => this.convText(el))
      this.text = this.messages[0]
      this.ticker()
    }
  }
  </script>
  
  <style scoped>
  .title {
    min-width: 0.3em;
    font-size: 5rem;
  }
  .item {
    display: inline-block;
    min-width: 0.3em;
    font-size: 5rem;
    animation: text-in .8s cubic-bezier(0.22, 0.15, 0.25, 1.43) 0s backwards;
  }
  /* 트랜지션 전용 스타일 */
  .v-enter-active,
  .v-leave-active,
  .v-move {
    transition: all 1s;
  }
  .v-leave-active {
    position: absolute;
  }
  .v-enter,
  .v-leave-to {
    opacity: 0;
    transform: translateY(-30px);
  }
  </style>