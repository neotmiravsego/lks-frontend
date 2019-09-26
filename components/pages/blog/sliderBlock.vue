<template lang="pug">
  .slider__blog
    .slider__blog__img__wrap
      img(src="../../../assets/images/blogslider.png",).slider__img
    .slider__blog__content
      .slider__blog__title__wrap
        h2.slider__blog__title {{slideData.title}}
      .slider__blog__txt__wrap
        p.slider__blog__txt__data {{slideData.created_at}}<br>
         <span class="slider__data__time">{{time}}</span>
        p.slider__blog__txt(v-html="slideData.content")
        p.slider__blog__author(v-if="slideData.author") <span class="slider__author__txt">Автор:</span> {{slideData.author}}
      .button__slide__wrap
        button.slide__button Читать
</template>

<script>
export default {
  props: {
    slideData: {}
  },
  data() {
    return {
      time: '17:59'
    }
  }
}
</script>

<style lang="scss" scoped>
.slider__blog {
  margin-bottom: 40px;
  display: flex;
  color: black;
  @include md {
    display: flex;
    flex-direction: column;
  }
  .slider__blog__img__wrap {
    margin-right: 58px;
    @include md {
      margin-right: 0;
    }
    .slider__img {
      display: block;
      object-fit: cover;
      @include md {
        width: 100%;
        height: 488px;
      }
    }
  }
  .slider__blog__content {
    .button__slide__wrap {
      display: flex;
      justify-content: flex-end;
      .slide__button {
        background: #e0c0c3;
        box-shadow: 0px 4px 20px rgba(0, 0, 0, 0.1);
        border-radius: 30px;
        padding: 11px 46px;
        font-size: $fontSize3;
        color: $white;
      }
    }
    .slider__blog__title__wrap {
      margin-bottom: 10px;
      max-width: 438px;
      width: 100%;
      line-height: $lineHeight4;
    }
    .slider__blog__author {
      font-size: $fontSize1;
      .slider__author__txt {
        font-weight: bold;
      }
    }
    .slider__blog__txt__wrap {
      margin-bottom: 30px;
      width: 100%;
      font-size: $fontSize4;
      line-height: 28px;
      text-align: justify;
      max-height: 270px;
      overflow: hidden;
      .slider__blog__txt {
        margin-bottom: 17px;
      }
      .slider__blog__txt__data {
        margin-bottom: 16px;
        display: block;
        font-size: $fontSizesm;
        color: $neutral;
        line-height: 17px;
      }
    }
  }
}
</style>
