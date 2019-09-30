<template lang="pug">
  header.header__component
    img(src="../../assets/images/HeaderBgImg.png", alt="alt").header__bg__img
    .header__wrap
      .header__title__wrap
        p.header__label Блог и магазин по вязанию
        h1.header__title Little Kniths Story
      .header__bottom__bar
        .header__socials
          ul.header__socials__list
            li.header__socials__list__item
              a(href="#").header__socials__link.facebook
                img.headerSocial__img(src="../../assets/images/svg/vk.svg")
            li.header__socials__list__item
              a(href="#").header__socials__link.facebook
                img.headerSocial__img(src="../../assets/images/svg/facebook.svg")
            li.header__socials__list__item
              a(href="#").header__socials__link.facebook
                img.headerSocial__img(src="../../assets/images/svg/instagram.svg")
            li.header__socials__list__item
              a(href="#").header__socials__link.facebook
                img.headerSocial__img(src="../../assets/images/svg/lid.svg")
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
                img.header__controls__img(src="../../assets/images/svg/login.svg")
            li.header__controls__list__item
              a(href="#").header__controls__link
                img.header__controls__img(src="../../assets/images/svg/shopping-bag.svg")
            li.header__controls__list__item
              a(href="#").header__controls__link
                img.header__controls__img(src="../../assets/images/svg/heart-shape-outline.svg")
    .header__button__lang
      button.header__button Ru
</template>

<script>
</script>

<style lang="scss" scoped src="./index.scss">
</style>
