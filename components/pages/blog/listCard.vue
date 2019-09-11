  <template lang="pug">
    li.other__blog__card__item
      a(href="#").other__blog__card__link
        .other__blog__card__content
          .other__blog__card__img__wrap
            img(src="../../../assets/images/otherBlogs.png", alt="alt").other__blog__card__img
          p.other__blog__card__data 13 ноября 2018 г. 17:56
          .other__blog__card__txt__wrap
            p.other__blog__card__title White shark monkeyface prickleback bluefish kuhli loach; large-e
            p.other__blog__card__txt__wrap
              | Сайт рыбатекст поможет дизайнеру, верстальщику,
              | вебмастеру сгенерировать несколько абзацев более менее осмысленного текста 
</template>

<style lang="scss" scoped>
.other__blog__card__item {
  margin-bottom: 114px;
  padding: 0 15px;
  width: 33.3%;
  box-sizing: border-box;
}
.other__blog__card__img {
  width: 100%;
}
.other__blog__card__img__wrap {
  margin-bottom: 16px;
}
.other__blog__card__txt__wrap {
  font-size: $fontSize3;
  line-height: 25px;
  text-align: center;
  text-align: center;
}
.other__blog__card__data {
  margin-left: 12px;
  margin-bottom: 16px;
  color: $neutral;
}
.other__blog__card__title {
  margin-bottom: 16px;
  font-weight: bold;
}
// ===media lg==
.other__blog__card__item {
  @include lg {
    margin-bottom: 80px;
    width: 50%;
    padding: 0 25px;
  }
}
// ===media md===
.other__blog__card__item {
  @include md {
    width: 100%;
    padding: 0;
  }
}
.other__blog__card__title {
  @include md {
    font-size: $fontSize2;
  }
}
.other__blog__card__txt__wrap {
  @include md {
    font-size: $fontSize1;
  }
}
.other__blog__card__item {
  @include md {
    margin-bottom: 60px;
  }
}
</style>
