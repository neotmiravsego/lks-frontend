<template lang="pug">
  header.header__component
    .header__wrap
      .header__title__wrap
        p.header__label Блог и магазин по вязанию
        h1.header__title Little Kniths Story
      .header__bottom__bar
        .header__socials
          ul.header__socials__list
            li.header__socials__list__item
              a(href="#").header__socials__link.facebook
                img.headerSocial__img(src="../assets/images/svg/vk.svg")
            li.header__socials__list__item
              a(href="#").header__socials__link.facebook
                img.headerSocial__img(src="../assets/images/svg/facebook.svg")
            li.header__socials__list__item
              a(href="#").header__socials__link.facebook
                img.headerSocial__img(src="../assets/images/svg/instagram.svg")
            li.header__socials__list__item
              a(href="#").header__socials__link.facebook
                img.headerSocial__img(src="../assets/images/svg/lid.svg")
        nav.navigation__header
          ul.navigation__list
            li.navigation__list__item
              a(href="#").navigation__list__item__link блог
            li.navigation__list__item
              a(href="#").navigation__list__item__link магазин
            li.navigation__list__item
              a(href="#").navigation__list__item__link авторы
            li.navigation__list__item
              a(href="#").navigation__list__item__link контакты
            li.navigation__list__item
              a(href="#").navigation__list__item__link схемы
        .header__controls
          ul.header__controls__list
            li.header__controls__list__item
              a(href="#").header__controls__link
                img.header__controls__img(src="../assets/images/svg/login.svg")
            li.header__controls__list__item
              a(href="#").header__controls__link
                img.header__controls__img(src="../assets/images/svg/shopping-bag.svg")
            li.header__controls__list__item
              a(href="#").header__controls__link
                img.header__controls__img(src="../assets/images/svg/heart-shape-outline.svg")
    .header__button__lang
      button.header__button
</template>

<style lang="scss" scoped>
.header__component {
  margin-bottom: 32px;
  .header {
    position: relative;
    &__wrap {
      margin: 0 auto;
      padding: 40px 0 0;
      width: 100%;
      max-width: $widthContainer1;
      text-align: center;
      font-size: $fontSize1;
    }
    &__label {
      margin-bottom: 16px;
    }
    &__title {
      font-size: 36px;
      text-transform: uppercase;
      color: #8a8e99;
      &__wrap {
        margin-bottom: 60px;
      }
    }
  }
  .header__socials {
    &__list {
      display: flex;
      align-items: center;
      &__item {
        padding: 0 14px;
      }
    }
  }
  .navigation__header {
    padding: 0 20px;
    .navigation__list {
      margin: 0 -20px;
      display: flex;
      &__item {
        padding: 0 20px;
        text-transform: uppercase;
        &:last-child {
          margin-right: 0;
        }
        @include lg {
          padding: 0 10px;
          &__link {
            font-size: 12px;
          }
        }
      }
    }
  }
  .header__controls {
    .header__controls__list {
      display: flex;
      align-items: center;
    }
    .header__controls__list__item {
      padding: 0 25px;
    }
    .header__controls__list__item:last-child {
      margin-right: 0;
    }
  }
  .header__bottom__bar {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: space-between;
  }
  .header__button__lang {
    position: absolute;
    right: 20px;
    top: 0;
    width: 50px;
    height: 50px;
    .header__button {
      width: 100%;
      height: 100%;
      background: #e0c0c3;
    }
  }
  // ===media lg==
  @include lg {
    padding: 40px 20px 0;
  }
  .header__socials__list__item {
    @include lg {
      padding: 0 20px;
    }
  }
  .header__controls {
    @include lg {
      .header__controls__list__item {
        padding: 0 10px;
      }
    }
  }
  // ====media xs===
  .header__controls__list {
    .header__controls__list__item {
      @include xs {
        padding: 0 20px;
      }
    }
  }
  .navigation__list {
    @include xs {
      margin: 0 -15px;
      &__item {
        padding: 0 15px;
      }
    }
  }
  // ===media md===
  .header__button__lang {
    @include md {
      height: 25px;
      width: 25px;
    }
  }
  .header__title {
    @include md {
      font-size: $fontSize5;
    }
  }
  .header__title__wrap {
    @include md {
      margin-bottom: 20px;
    }
  }
  .header__socials {
    @include md {
      margin-bottom: 20px;
      &__list {
        @include md {
          justify-content: center;
        }
      }
      &__item {
        @include md {
          margin-right: 10px;
        }
      }
    }
  }
  .header__bottom__bar {
    @include md {
      display: block;
    }
  }
  .navigation__list {
    @include md {
      margin-bottom: 20px;
      flex-wrap: wrap;
      justify-content: center;
      font-size: 12px;
      &__item {
        line-height: 20px;
        padding: 0 10px;
      }
    }
  }
  .header__controls__list {
    @include md {
      justify-content: center;
      margin: 0;
      padding: 0 20px;
    }
  }
}
</style>
