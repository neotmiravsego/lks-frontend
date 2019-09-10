<template lang="pug">
  header
    .header__component
      .header__title__wrap
        p.header__label Блог и магазин по вязанию
        h1.header__title Little Kniths Story
      .header__bottom__bar
        .header__socials
          ul.header__socials__list
            li.header__social__list__item
              a(href="#").header__social__link.facebook
                img.headerSocial__img(src="../assets/images/svg/vk.svg")
            li.header__social__list__item
              a(href="#").header__social__link.facebook
                img.headerSocial__img(src="../assets/images/svg/facebook.svg")
            li.header__social__list__item
              a(href="#").header__social__link.facebook
                img.headerSocial__img(src="../assets/images/svg/instagram.svg")
            li.header__social__list__item
              a(href="#").header__social__link.facebook
                img.headerSocial__img(src="../assets/images/svg/lid.svg")
        nav.navigation
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
.header {
  position: relative;
}
.header__component {
  margin: 0 auto;
  margin-bottom: 32px;
  padding: 40px 0 0;
  width: 100%;
  max-width: 1111px;
  text-align: center;
  font-size: $fontSize1;
}
.header__label {
  margin-bottom: 16px;
  font-family: $ffFranc;
}
.header__title {
  font-size: 36px;
  text-transform: uppercase;
  color: #8a8e99;
}
.header__title__wrap {
  margin-bottom: 45px;
}
.header__socials__list {
  display: flex;
  align-items: center;
}
.header__social__list__item {
  margin-right: 28px;
}
.header__social__list__item:last-child {
  margin-right: 0;
}
.navigation__list {
  display: flex;
}
.navigation__list__item {
  margin-right: 40px;
  text-transform: uppercase;
  font-family: $ffFranc;
}
.navigation__list__item:last-child {
  margin-right: 0;
}
.header__controls__list {
  display: flex;
  align-items: center;
}
.header__controls__list__item {
  margin-right: 50px;
}
.header__controls__list__item:last-child {
  margin-right: 0;
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
}
.header__button {
  width: 100%;
  height: 100%;
  background: orange;
}
</style>
