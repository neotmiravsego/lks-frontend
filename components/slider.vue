<template lang="pug">
  .slider
    p {{news}}
    .slider__wrap(ref="sliderWrap")
      ul.slider__line(ref="sliderLine")
        li.slider__line__item(v-for="item of news")
          SliderBlock.slide(:slideData="item")
    .slider__controls__panel
      ul.slider__controls__list
        li.slider__controls__list__item
          span.slider__controls__dot
        li.slider__controls__list__item
          span.slider__controls__dot
        li.slider__controls__list__item
          span.slider__controls__dot
        li.slider__controls__list__item
          span.slider__controls__dot
        li.slider__controls__list__item
          span.slider__controls__dot
        li.slider__controls__list__item
          span.slider__controls__dot
        li.slider__controls__list__item
          span.slider__controls__dot
      .slider__button__position__wrap
        button.slider__controls__button__left(ref="prev")
          img(src="../assets/images/Rectangle-left.png", alt="alt")
        button.slider__controls__button__right#next(ref="next")
          img(src="../assets/images/Rectangle-right.png", alt="alt").controls__button__right
        button.slider__controls__button__read Читать
</template>

<script lang="JavaScript">
import SliderBlock from '~/components/pages/blog/sliderBlock.vue'

export default {
  components: {
   SliderBlock
  },
  data () {
    return {
      offset: 0,
      news: []
    }
  },
  // такуюже offset = x
  mounted() {
    this.createSlider()
    window.addEventListener('resize', this.resize)
    this.getData()
  },
  destroyed() {
    window.removeEventListener('resize', this.resize)
  },
  methods: {
    getData() {
      fetch('http://dev.backend.littleknitsstory.com/api/posts/',{
        method: 'GET'
      }).then((response) => {
              /* eslint-disable */
        return response.json()
      }).then((json) => {
        this.news=json
        this.createSlider()
      })
    },
    // вынести в блоg
    //создать data
    createSlider () {
      const { prev, next, sliderLine, sliderWrap } = this.$refs
      const lineWidth = sliderWrap.offsetWidth + 40;
      const slidesCount = this.news.length - 1;
      let { offset } = this

      function prevHandler() {
        if (offset < 0) {
          offset = offset + lineWidth;
          sliderLine.style.left = offset +'px';
        }
      }

      function nextHandler() {
        console.log(lineWidth)
        if (offset <= -(slidesCount*lineWidth)) {
            return;
        }
        offset = offset - lineWidth;
        sliderLine.style.left = offset + 'px';
      }

      prev.onclick = prevHandler
      next.onclick = nextHandler
    },
    resize(){
      /* eslint-disable */
       this.createSlider();
    }
  }
}
</script>

<style lang="scss" scoped>
.slider {
  position: relative;
  margin: 0 auto;
  margin-bottom: 40px;
  width: 100%;
  max-width: $widthContainer1;
  &__wrap {
    overflow: hidden;
  }
  &__line {
    display: flex;
    position: relative;
    transition: all ease 1s;
    left: 0;
    &__item {
      margin-right: 40px;
      width: 100%;
      flex-shrink: 0;
      &:last-child {
        margin-right: 0;
      }
    }
    &::after {
      content: '';
      display: block;
      clear: both;
    }
  }
  // overflow: hidden;
  .slider__controls__panel {
    width: 100%;
    max-width: 699px;
    display: flex;
    position: absolute;
    right: 0;
    bottom: 0;
    justify-content: space-between;
    align-items: center;
    .slider__controls__list {
      display: flex;
      .slider__controls__dot {
        display: block;
        margin-left: 10px;
        width: 7px;
        height: 7px;
        border: 1px solid $neutral;
        border-radius: 50%;
      }
    }
  }
  .slider__button__position__wrap {
    .slider__controls__button__left {
      margin-right: 18px;
      width: 30px;
      height: 40px;
      border-radius: 20px;
      background: $white;
      &:hover {
        background: linear-gradient(90deg, $light 50%, transparent 50%);
      }
    }
    .slider__controls__button__right {
      margin-right: 40px;
      width: 30px;
      height: 40px;
      border-radius: 20px;
      background: $white;
      &:hover {
        background: linear-gradient(270deg, $light 50%, transparent 50%);
      }
    }
    .slider__controls__button__read {
      padding: 11px 50px;
      font-size: $fontSize2;
      color: $white;
      background: #e0c0c3;
      box-shadow: 0px 4px 20px rgba(0, 0, 0, 0.1);
      border-radius: 30px;
    }
  }
}
</style>
