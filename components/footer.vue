<template lang="pug">
    footer
      .footer__component__top__bar
        .footer__panel
          .footer__panel__navigation__wrap
            h3.footer__panel__navigation__title Навигация
            ul.footer__panel__navigation__list
              li.footer__panel__navigation__item
                a(href="#").footer__panel__navigation__link Блог
              li.footer__panel__navigation__item
                a(href="#").footer__panel__navigation__link Магазин
              li.footer__panel__navigation__item
                a(href="#").footer__panel__navigation__link О нас
              li.footer__panel__navigation__item
                a(href="#").footer__panel__navigation__link Портфолио
              li.footer__panel__navigation__item
                a(href="#").footer__panel__navigation__link Контакты
          .footer__panel__controls__wrap
            h3.footer__panel__controls__title Личный кабинет
            ul.footer__panel__controls__list
              li.footer__panel__controls__item
                a(href="#").footer__panel__controls__link Войти
              li.footer__panel__controls__item
                a(href="#").footer__panel__controls__link Корзина
              li.footer__panel__controls__item
                a(href="#").footer__panel__controls__link Сохраненные товары
        form.footer__form
          input.footer__input(
            type='sumbit'
            placeholder='Ваш E-mail'
            )
          button.footer__button Подписаться
          .footer__form__txt__wrap
            p.footer__form__txt
              | Мы проводим специальные акции для наших клиентов.
              | оформите подписку и мы будем держать вас в курсе
        .footer__social__list__wrap
          ul.footer__social__list
            li.footer__social__list__item
              a(href="#").footer__social__item__link
                img(src="../assets/images/svg/fbFooter.svg", alt="alt")
            li.footer__social__list__item
              a(href="#").footer__social__item__link
                img(src="../assets/images/svg/instagramFooter.svg", alt="alt")
            li.footer__social__list__item
              a(href="#").footer__social__item__link
                img(src="../assets/images/svg/vkFooter.svg", alt="alt")
            li.footer__social__list__item
              a(href="#").footer__social__item__link
                img(src="../assets/images/svg/prsFooter.svg", alt="alt")
      .footer__component__bottom__bar__wrap
        .footer__component__bottom__bar
          .copyright__wrap Little Knits Story 2017 | All Rights Reserved
          .footer__logo
            img(src="../assets/images/logo_footer.png", alt="alt").footer__logo__img
          .privacy__policy
            a(href="#").privacy__policy__link Политика конфеденциальности

</template>

<style lang="scss">
footer {
  border: 1px solid #e5e5e5;
}
.footer__component__top__bar {
  padding: 24px 0;
  margin: 0 auto;
  width: 100%;
  max-width: 1100px;
}
.footer__panel {
  margin-bottom: 40px;
  display: flex;
  justify-content: space-between;
}
.footer__form {
  margin: 0 auto;
  position: relative;
  width: 100%;
  max-width: 950px;
}
.footer__input {
  margin-bottom: 16px;
  width: 100%;
  height: 30px;
  max-width: 950px;
  border-radius: 20px;
  outline: none;
  border: none;
  background: #f0f0f0;
}
.footer__panel__navigation__title {
  margin-bottom: 18px;
}
.footer__panel__navigation__list {
  display: flex;
}
.footer__panel__navigation__item {
  padding-right: 40px;
}
.footer__panel__navigation__item:last-child {
  padding-right: 0;
}
.footer__panel__controls__list {
  display: flex;
}
.footer__panel__controls__title {
  margin-bottom: 16px;
}
.footer__panel__controls__item {
  padding-right: 40px;
}
.footer__panel__controls__item:last-child {
  padding-right: 0px;
}
.footer__input {
  padding: 0 10px;
}
.footer__button {
  padding: 6px 50px;
  position: absolute;
  right: 0;
  border-radius: 20px;
  outline: none;
  border: none;
  background: #e0c0c3;
  color: #fff;
  font-size: $fontSize2;
}
.footer__form__txt__wrap {
  margin: 0 auto;
  margin-bottom: 24px;
  width: 100%;
  max-width: 622px;
  text-align: center;
  color: $neutral;
}
.footer__social__list {
  display: flex;
  justify-content: center;
}
.footer__social__list__item {
  padding-right: 32px;
}
.footer__social__list__item:last-child {
  padding-right: 0;
}
.footer__component__bottom__bar {
  margin: 0 auto;
  padding: 20px 400px 32px;
  display: flex;
  flex-wrap: wrap;
  border: 1px solid #e5e5e5;
  align-items: center;
  justify-content: space-between;
  color: $neutral;
}
.privacy__policy__link {
  color: $neutral;
}
</style>
