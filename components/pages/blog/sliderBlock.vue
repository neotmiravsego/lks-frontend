<template lang="pug">
  .slider__blog
    .slider__blog__img__wrap
      img(src="../../../assets/images/blogslider.png",).slider__img
    .slider__blog__content
      .slider__blog__title__wrap
        h2.slider__blog__title White shark monkeyface prickleback bluefish kuhli loach; large-e
      .slider__blog__txt__wrap
        p.slider__blog__txt__data 13 ноября 2018 г.<br>
         <span class="slider__data__time">17:56</span>
        p.slider__blog__txt 
          | Сайт рыбатекст поможет дизайнеру, верстальщику,
          | вебмастеру сгенерировать несколько абзацев более менее осмысленного текста рыбы на русском языке,
          | а начинающему оратору отточить навык публичных выступлений в домашних условиях.
        p.slider__blog__author <span class="slider__author__txt">Автор:</span> Катя Анаприенко
</template>
<style lang="scss" scoped>
.slider__blog {
  display: flex;
  color: black;
  .slider__blog__img__wrap {
    margin-right: 58px;
    .slider__img {
      display: block;
      object-fit: cover;
    }
  }
  .slider__blog__content {
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
      width: 100%;
      font-size: $fontSize4;
      text-align: justify;
      line-height: 28px;
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
