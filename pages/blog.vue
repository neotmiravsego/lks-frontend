<template lang="pug">
  .container__blog
    vHeader
    breadCrumbs
    .blog__container
      vSlider
      ul.blog__list
        listCard.blog__list__card
        listCard.blog__list__card
        listCard.blog__list__card
        listCard.blog__list__card
        listCard.blog__list__card
        listCard.blog__list__card
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

<style lang="scss" scoped>
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
  .blog__list__card {
    width: 33.3%;
    border-radius: 10px;
    padding: 0 15px;
  }
}
</style>
