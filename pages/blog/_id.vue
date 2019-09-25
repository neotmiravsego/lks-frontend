<template lang="pug">
  .container
    vHeader
    breadCrumbs
    vSectionContent(:newsData="newsData")
    section.other__blogs
      h3.other__blogs__title Другие блоги
      ul.other__blogs__list
        listCard.other__blogs__list__card
        listCard.other__blogs__list__card
        listCard.other__blogs__list__card
        listCard.other__blogs__list__card
        listCard.other__blogs__list__card
        listCard.other__blogs__list__card
    vFooter
    
</template>

<script>
import vHeader from '~/components/header/index.vue'
import vSectionContent from '~/components/sectionContent.vue'
import listCard from '~/components/pages/blog/listCard.vue'
import breadCrumbs from '~/components/pages/blog/breadCrumbs.vue'
import vFooter from '~/components/footer/index.vue'

export default {
  components: {
    vHeader,
    vSectionContent,
    listCard,
    breadCrumbs,
    vFooter
  },
  data() {
    return {
      newsData: {}
    }
  },
  mounted() {
    this.getData()
  },
  methods: {
    getData() {
      const { id } = this.$route.params
      fetch(`http://dev.backend.littleknitsstory.com/api/posts/${id}`, {
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
.container {
  margin: 0 auto;
  width: 100%;
  .other__blogs {
    margin: 0 auto;
    width: 100%;
    max-width: 1110px;
    @include lg {
      max-width: 700px;
    }
    @include md {
      max-width: 320px;
    }
  }
  .other__blogs__list {
    margin: 0 -15px;
    display: flex;
    flex-wrap: wrap;
    &__card {
      width: 33.33%;
      padding: 0 15px;
      margin-bottom: 32px;
    }
    @include lg {
      margin: 0 -25px;
    }
    @include md {
      margin: 0;
      padding: 0 10px;
    }
  }
  .other__blogs__title {
    margin-bottom: 24px;
    @include lg {
      text-align: center;
    }
    @include md {
      text-align: center;
    }
  }
}
</style>
