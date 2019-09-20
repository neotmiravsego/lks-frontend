<template lang="pug">
  .section__content__component
    img(src="../assets/images/OtherImg.png", alt="alt").content__bg__img__right
    img(src="../assets/images/OtherImg.png", alt="alt").content__bg__img__left
    .section__content
      .section__content__title__wrap
        h2.section___content__title White shark monkeyface prickleback bluefish kuhli loach; large-e
      .blog__author
        .content__data__author
          p.content__data
           span.content__data__time 13 ноября 2018 г.<br> 17:56
          p.content__author <span class="author__txt">Автор:</span> Катя Анаприенко
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
  position: relative;
  .content__bg__img__right {
    position: absolute;
    right: 328px;
    @include lg {
      right: 0;
    }
    @include md {
      right: 50px;
    }
  }
  .content__bg__img__left {
    position: absolute;
    left: 326px;
    top: 300px;
    @include md {
      left: 50px;
      top: 600px;
    }
  }
  .section__content {
    position: relative;
    margin: 0 auto;
    width: 100%;
    max-width: $widthContainer2;
    &_title {
      @include md {
        line-height: $lineHeight1;
      }
    }
    @include lg {
      padding: 0 50px;
      &__title {
        line-height: $lineHeight3;
      }
    }
    @include md {
      padding: 0 40px;
    }
    @include xs {
      padding: 0 10px;
    }
  }
  .blog__author__txt__wrap {
    padding: 0 50px;
    margin-bottom: 40px;
    width: 100%;
    text-align: justify;
  }
  .content__author {
    font-size: $fontSize1;
  }
  .content__data {
    color: $neutral;
    margin-bottom: 15px;
    @include lg {
      margin-bottom: 5px;
    }
    &__author {
      margin-left: 56px;
      margin-bottom: 24px;
      line-height: 24px;
      @include lg {
        font-size: $fontSize1;
      }
      @include md {
        margin: 0 0 20px;
      }
    }
    @include md {
      margin: 0 0 10px;
      font-size: $fontSize1;
      line-height: $lineHeight1;
    }
  }
  .section__content__title__wrap {
    padding: 0 40px;
    margin-bottom: 16px;
    width: 100%;
    text-align: center;
    line-height: $lineHeight4;
    @include md {
      line-height: $lineHeight1;
    }
  }
  .blog__author {
    position: relative;
    font-size: $fontSize4;
    &__txt {
      line-height: $lineHeight3;
      font-family: $ffHelv;
      @include lg {
        padding: 0 20px;
        font-size: $fontSize2;
      }
      @include md {
        font-size: $fontSize1;
        line-height: $lineHeight2;
        &__wrap {
          padding: 0;
        }
      }
    }
    &__img__wrap {
      width: 100%;
      margin-bottom: 24px;
    }
    &__img {
      width: 100%;
    }
    &__top__txt {
      margin-bottom: 50px;
      @include md {
        margin: 0 0 20px;
      }
    }
    &__comment {
      margin-bottom: 16px;
      width: 100%;
      text-align: left;
      @include lg {
        font-size: $fontSize3;
      }
      @include md {
        font-size: $fontSize2;
      }
    }
  }
  .author__img__bottom__wrap {
    margin-bottom: 12px;
  }
  .other__blogs__author__title {
    margin-bottom: 16px;
    line-height: $lineHeight3;
    @include md {
      line-height: $lineHeight2;
    }
  }
}
</style>
