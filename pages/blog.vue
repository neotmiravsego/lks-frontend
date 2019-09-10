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
  widows: 100%;
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
</style>
