<template>
  <section class="newProjectPC">
    <div class="contentTtlPcWithoutPic">
      <p class="contentTtlPcWithoutPic__sub">New Projects</p>
      <h3 class="contentTtlPcWithoutPic__main">新着案件</h3>
    </div>
    <div class="linkCardList">
      <!-- <button type="button" class="linkCardList__btn linkCardList__btn__back"></button> -->
      <div class="linkCardList__slider">
        <input type="radio" name="cs_anchor1" id="cs_slider1_0" class="cs_anchor slide">
        <input type="radio" name="cs_anchor1" id="cs_slider1_1" class="cs_anchor slide">
        <input type="radio" name="cs_play1" id="cs_slider1_1" class="cs_anchor">
        <input type="radio" name="cs_pause1" id="cs_slider1_1" class="cs_anchor">
        <ul class="projects">
          <div style="width: 100%; visibility: hidden; font-size: 0px; line-height: 0;">
            <div style="width: 100%;"></div>
          </div>
          <li class="num0 projects__group">
            <a href="#" class="projects__group__item project">
              <div class="project__ttl">[Java]オンライン資格系システム開発の求人・案件</div>
              <div class="project__content">
                <div class="project__content__payment">~<span>750,000</span>円/月</div>
                <div class="project__content__contractType">業務委託</div>
                <div class="project__content__infrastructure">AWS, Java</div>
                <div class="project__content__place">新橋(東京都)</div>
              </div>
            </a>
          </li>
          <li class="num1 projects__group">
            <a href="#" class="eachProject">
              <div class="eachProject__ttl">[Java]オンライン資格系システム開発の求人・案件</div>
              <div class="eachProject__content">
                <div class="eachProject__content__payment">~<span>750,000</span>円/月</div>
                <div class="eachProject__content__contractType">業務委託</div>
                <div class="eachProject__content__infrastructure">AWS, Java</div>
                <div class="eachProject__content__place">新橋(東京都)</div>
              </div>
            </a>
          </li>
        </ul>
        <div class="cs_arrowPrev">
          <label for="cs_slide1_0" class="num0"></label>
          <label for="cs_slide1_1" class="num1"></label>
          <label for="cs_slide1_2" class="num2"></label>
        </div>
        <div class="cs_arrowNext">
          <label for="cs_slide1_0" class="num0"></label>
          <label for="cs_slide1_1" class="num1"></label>
          <label for="cs_slide1_2" class="num2"></label>
        </div>
        <div class="cs_bullets">
          <label for="cs_slide1_0" class="num0"></label>
          <label for="cs_slide1_1" class="num1"></label>
          <label for="cs_slide1_2" class="num2"></label>
        </div>
      </div>
        <!-- <div class="linkCardList__slider__item eachProject">
          <div class="eachProject__ttl">[Java]オンライン資格系システム開発の求人・案件</div>
          <div class="eachProject__content">
            <div class="eachProject__content__payment">~<span>750,000</span>円/月</div>
            <div class="eachProject__content__contractType">業務委託</div>
            <div class="eachProject__content__infrastructure">AWS, Java</div>
            <div class="eachProject__content__place">新橋(東京都)</div>
          </div>
        </div>
      </div>
      <button type="button" class="linkCardList__btn linkCardList__btn__next"></button>
      <ul class="sliderCorrespondedBtn">
        <li>
          <button type="radio"></button>
          <button type="radio"></button>
          <button type="radio"></button>
        </li>
      </ul> -->
    </div>
    <div class="newJobs">
      <a href="#" class="newJobs__link">全ての新着案件を見る</a>
    </div>
  
  </section>
</template>

<script>
</script>

<style lang="scss" scoped>
@import '../assets/style/global/_color';
@import '../assets/style/global/_border';
@import '../assets/style/global/_sectionDefault';

.newProjectPC {
  @extend %sectionDefault;
}

.linkCardList__slider {
  position: inline-block;
  display: inline-block;
  width: 100%;
  margin-top: 10px; 
  .cs_anchor {
    display: none;
  }
}

.projects {
  // position: relative;
  // z-index: 1;
  // font-size: 0;
  // line-height:0;
  // padding: 0;
  // margin: 0 auto;
  // overflow: hidden;
  // white-space: nowrap;
  &__group {
    display: flex;
    &__item {
      width: 25%;
    }
  }
}

.project {

}

</style>