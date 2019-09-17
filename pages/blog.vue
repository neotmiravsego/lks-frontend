<template lang="pug">
  .container__blog
    vHeader
    breadCrumbs
    .blog__container
      vSlider
      ul.blog__list
        listCard.card__blog__list
        listCard.card__blog__list
        listCard.card__blog__list
        listCard.card__blog__list
        listCard.card__blog__list
        listCard.card__blog__list
    vFooter
</template>

<script>
import vHeader from '~/components/header/index.vue'
import listCard from '~/components/pages/blog/listCard.vue'
import breadCrumbs from '~/components/pages/blog/breadCrumbs.vue'
import vFooter from '~/components/footer/index.vue'
import vSlider from '~/components/slider.vue'
import '../assets/scss/mixins.scss'

export default {
  components: {
    vHeader,
    listCard,
    breadCrumbs,
    vFooter,
    vSlider
  }
}
</script>

<style lang="scss">
.container__blog {
  .blog__container {
    width: 100%;
    max-width: $widthContainer1;
    margin: 0 auto;
  }
  .blog__list {
    margin: 0 -15px;
    display: flex;
    flex-wrap: wrap;
  }
  .other__blog__card__item {
    width: 33.3%;
    border-radius: 10px;
    &:hover {
      box-shadow: 20px 10px 30px rgba(0, 0, 0, 0.15);
      .card__button {
        display: block;
      }
    }
  }
}
</style>
