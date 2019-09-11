<template lang="pug">
  .section__content__component
    .section__content
      .section__content__title__wrap
        h2.section___content__title White shark monkeyface prickleback bluefish kuhli loach; large-e
      .content__data__author
        p.content__data
          span.content__data__time 13 ноября 2018 г.<br> 17:56
        p.content__author <span class="author__txt">Автор:</span> Катя Анаприенко
      .blog__author
        .blog__author__txt__wrap
          p.blog__author__txt
            | Таким образом постоянный количественный рост и сфера нашей активности позволяет выполнять важные задания по разработке существенных финансовых и административных условий.
            | Значимость этих проблем настолько очевидна, что начало повседневной работы по формированию позиции способствует подготовки и реализации направлений прогрессивного развития.
            | Повседневная практика показывает, что реализация намеченных плановых заданий позволяет выполнять важные задания по разработке позиций, занимаемых участниками в отношении поставленных задач.
            | Идейные соображения высшего порядка, а также начало повседневной работы по формировани
        .blog__author__img__wrap
          img(src="../assets/images/authorImage.png", alt="alt").blog__author__img
        .blog__author__txt__wrap
          p.blog__author__txt
            | Повседневная практика показывает, что постоянное информационно-пропагандистское обеспечение нашей деятельности требуют определения и уточнения позиций, занимаемых участниками в отношении поставленных задач. 
            | Задача организации, в особенности же новая модель организационной деятельности требуют от нас анализа новых предложений. Разнообразный и богатый опыт консультация с широким активом требуют определения и уточнения систем массового участия.
            | Товарищи! новая модель организационной деятельности обеспечивает широкому кругу (специалистов) участие в формировании систем массового участия.
            | Товарищи! постоянный количественный рост и сфера нашей активности требуют от нас анализа системы обучения кадров, соответствует насущным потребностям.
        .blog__author__img__wrap.author__img__bottom__wrap
          img(src="../assets/images/authorImage.png", alt="alt").blog__author__img
        p.blog__author__comment Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
        .other__blogs__author.blog__author__txt__wrap
          h3.other__blogs__author__title 
            | Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
            | Aenean commodo ligula eget dolor.
          p.blog__author__txt
            | Задача организации, в особенности же укрепление и развитие структуры способствует подготовки и реализации направлений прогрессивного развития.
            | Товарищи! постоянное информационно-пропагандистское обеспечение нашей деятельности представляет собой интересный эксперимент проверки дальнейших направлений развития.
            | Идейные соображения высшего порядка, а также дальнейшее развитие различных форм деятельности требуют определения и уточнения системы обучения кадров, соответствует насущным потребностям.
            | Равным образом дальнейшее развитие различных форм деятельности способствует подготовки и реализации направлений прогрессивного развития.
        .other__blogs__author.blog__author__txt__wrap
          h3.other__blogs__author__title Lorem ipsum dolor sit amet, consectetuer adipiscing elit. 
          p.blog__author__top__txt.blog__author__txt
            | Разнообразный и богатый опыт рамки и место обучения кадров позволяет выполнять важные задания по разработке форм развития.
            | Не следует, однако забывать, что постоянное информационно-пропагандистское обеспечение нашей деятельности позволяет оценить значение существенных финансовых и административных условий.
            | С другой стороны реализация намеченных плановых заданий позволяет оценить значение соответствующий условий активизации.
          p.blog__author__txt
            | Повседневная практика показывает, что постоянное информационно-пропагандистское обеспечение нашей деятельности представляет собой интересный эксперимент проверки дальнейших направлений развития.
            | Разнообразный и богатый опыт дальнейшее развитие различных форм деятельности позволяет оценить значение позиций, занимаемых участниками в отношении поставленных задач.
</template>

<style lang="scss" scoped>
.section__content__component {
  .section__content {
    margin: 0 auto;
    width: 100%;
    max-width: 825px;
  }
  .blog__author__txt__wrap {
    margin-bottom: 40px;
    width: 100%;
    max-width: 710px;
    text-align: justify;
  }
  .content__data__time {
    color: #c4c4c4;
  }
  .content__data {
    margin-bottom: 15px;
  }
  .section__content__title__wrap {
    padding-bottom: 16px;
    width: 100%;
    max-width: 645px;
    margin: 0 auto;
    text-align: center;
  }
  .section___content__title {
    line-height: 50px;
  }
  .blog__author {
    display: flex;
    flex-direction: column;
    align-items: center;
    position: relative;
    font-size: $fontSize4;
  }
  .blog__author__txt {
    line-height: 40px;
  }
  .blog__author__img {
    width: 100%;
  }
  .blog__author__img__wrap {
    width: 100%;
    margin-bottom: 24px;
  }
  .author__img__bottom__wrap {
    margin-bottom: 12px;
  }
  .blog__author__top__txt {
    margin-bottom: 50px;
  }
  .content__data__author {
    margin-bottom: 24px;
    margin-left: 60px;
    line-height: 24px;
  }
  .blog__author__comment {
    margin-bottom: 16px;
    width: 100%;
    text-align: left;
  }
  .other__blogs__author__title {
    margin-bottom: 25px;
    line-height: 40px;
  }
  .other__blogs__author {
    margin-bottom: 25px;
  }
  // ==media lg===
  .section__content {
    @include lg {
      padding: 0 50px;
    }
  }
  .section___content__title {
    @include lg {
      line-height: 40px;
    }
  }
  .content__data__author {
    @include lg {
      font-size: $fontSize1;
    }
  }
  .content__data {
    @include lg {
      margin-bottom: 5px;
    }
  }
  .blog__author__txt {
    @include lg {
      padding: 0 20px;
      font-size: $fontSize2;
    }
  }
  .blog__author__comment {
    @include lg {
      font-size: $fontSize3;
    }
  }
  // ===media md===
  .section__content {
    @include md {
      max-width: 320px;
      padding: 0 8px;
    }
  }
  .section___content__title {
    @include md {
      line-height: 20px;
    }
  }
  .content__data__author {
    @include md {
      margin: 0 0 20px 20px;
    }
  }
  .blog__author__txt {
    @include md {
      font-size: $fontSize1;
      line-height: 25px;
    }
  }
  .blog__author__comment {
    @include md {
      font-size: $fontSize2;
    }
  }
  .other__blogs__author__title {
    @include md {
      line-height: 25px;
    }
  }
  .blog__author__top__txt {
    @include md {
      margin: 0 0 20px;
    }
  }
}
</style>
