<template lang="pug">
  .container__blog
    vHeader
    breadCrumbs
    .blog__container
      slideBlock(v-if="firstNews" :slideData="firstNews" )
      ul.blog__list
        listCard.blog__list__card(v-for="item of news" :key="item.id" :cardData="item")
      .button__watch__more__wrap
        button.button__more Cмотреть ещё
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
      news: [],
      firstNews: {}
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
          this.firstNews = json[0]
          this.news = json.filter(el => {
            return json[0].id !== el.id
          })
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
    padding: 0 20px;
  }
  .blog__list {
    margin: 0 -15px 82px;
    display: flex;
    flex-wrap: wrap;
    @include md {
      margin: 0;
    }
  }
  .blog__list__card {
    width: 33.3%;
    border-radius: 10px;
    padding: 0 15px;
    @include md {
      padding: 0;
      width: 100%;
    }
  }
  .button__watch__more__wrap {
    margin-bottom: 32px;
    text-align: center;
    .button__more {
      color: $dark;
      font-size: $fontSize3;
      border: none;
      outline: none;
      background: transparent;
    }
  }
}
</style>
