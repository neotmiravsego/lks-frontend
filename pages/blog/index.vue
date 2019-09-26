<template lang="pug">
  .container__blog
    vHeader
    breadCrumbs
    .blog__container
      slideBlock(v-if="news[0]" :slideData="news[0]")
      ul.blog__list
        listCard.blog__list__card(v-for="item of news" :key="item.id")
    vFooter
</template>

<script>
import slideBlock from '../../components/pages/blog/sliderBlock.vue'
import vHeader from '~/components/header/index.vue'
import listCard from '~/components/pages/blog/listCard.vue'
import breadCrumbs from '~/components/pages/blog/breadCrumbs.vue'
import vFooter from '~/components/footer/index.vue'
import vSlider from '~/components/slider.vue'

export default {
  components: {
    vHeader,
    listCard,
    breadCrumbs,
    vFooter,
    vSlider,
    slideBlock
  },

  data() {
    return {
      news: []
    }
  },
  mounted() {
    this.getData()
  },
  methods: {
    getData() {
      fetch('http://dev.backend.littleknitsstory.com/api/posts/', {
        method: 'GET'
      })
        .then(response => {
          return response.json()
        })
        .then(json => {
          this.news = json
        })
    }
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
