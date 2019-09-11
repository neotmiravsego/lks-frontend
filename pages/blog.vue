<template lang="pug">
  .container
    vHeader
    breadCrumbs
    vSectionContent
    section.other__blogs
      h3.other__blogs__title Другие блоги
      ul.other__blogs__list
        listCard
        listCard
        listCard
        listCard
        listCard
        listCard
    vFooter

</template>

<script>
import vHeader from '~/components/header.vue'
import vSectionContent from '~/components/sectionContent.vue'
import listCard from '~/components/pages/blog/listCard.vue'
import breadCrumbs from '~/components/pages/blog/breadCrumbs.vue'
import vFooter from '~/components/footer.vue'
import '../assets/scss/mixins.scss'

export default {
  components: {
    vHeader,
    vSectionContent,
    listCard,
    breadCrumbs,
    vFooter
  }
}
</script>

<style lang="scss">
.container {
  margin: 0 auto;
  width: 100%;
}
.other__blogs {
  margin: 0 auto;
  width: 100%;
  max-width: 1110px;
}
.other__blogs__list {
  margin: 0 -30px;
  display: flex;
  flex-wrap: wrap;
}
.other__blogs__title {
  margin-bottom: 24px;
}
// ===media lg==
.other__blog__list {
  @include lg {
    margin: 0 -25px;
  }
}
.other__blogs {
  @include lg {
    max-width: 700px;
  }
}
.other__blogs__title {
  @include lg {
    text-align: center;
  }
}
// ===media md==
.other__blogs__list {
  @include md {
    margin: 0;
  }
}
.other__blogs {
  @include md {
    max-width: 320px;
  }
}
.other__blogs__title {
  @include md {
    text-align: center;
  }
}
</style>
