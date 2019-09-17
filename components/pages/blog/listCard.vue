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
          button.card__button Читать
</template>

<style lang="scss" scoped>
.card__button {
  padding: 11px 46px;
  display: none;
  background: #e0c0c3;
  box-shadow: 0px 4px 20px rgba(0, 0, 0, 0.1);
  border-radius: 30px;
  font-size: $fontSize3;
  margin: 0 auto;
  color: #fff;
  letter-spacing: 1px;
  font-family: Helvetica;
}
.other__blog__card__item {
  margin-bottom: 114px;
  padding: 0 15px;
  width: 33.3%;
  box-sizing: border-box;
  @include lg {
    margin-bottom: 80px;
    width: 50%;
    padding: 0 25px;
  }
}
.other__blog__card__content {
  padding-bottom: 16px;
}
.other__blog__card__img {
  width: 100%;
}
.other__blog__card__img__wrap {
  margin-bottom: 16px;
}
.other__blog__card__txt__wrap {
  margin-bottom: 24px;
  font-size: $fontSize3;
  line-height: 25px;
  text-align: center;
  text-align: center;
  @include md {
    font-size: $fontSize1;
  }
}
.other__blog__card__data {
  margin-left: 12px;
  margin-bottom: 16px;
  color: $neutral;
}
.other__blog__card__title {
  margin-bottom: 16px;
  font-weight: bold;
  @include md {
    font-size: $fontSize2;
  }
}
// ===media lg==
.other__blog__card__item {
  @include lg {
    margin-bottom: 80px;
    width: 50%;
    padding: 0 25px;
  }
  @include md {
    margin-bottom: 60px;
  }
}
</style>
