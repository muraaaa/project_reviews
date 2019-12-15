<template>
  <div class="slider">
    <input type="radio" name="sliderRadio" class="sliderRadio" id="checkSlider1">
    <input type="radio" name="sliderRadio" class="sliderRadio" id="checkSlider2">
    <input type="radio" name="sliderRadio" class="sliderRadio" id="checkSlider3">
    <div class="slider__contents">
      <div class="slider__contents__content slider1">
        <label class="sliderLabel" for="checkSlider3">＜</label>
        No.1
        <label class="sliderLabel" for="checkSlider2">＞</label>
      </div>
      <div class="slider__contents__content slider2">
        <label class="sliderLabel" for="checkSlider1">＜</label>
        No.2
        <label class="sliderLabel" for="checkSlider3">＞</label>
      </div>
      <div class="slider__contents__content slider3">
        <label class="sliderLabel" for="checkSlider2">＜</label>
        No.3
        <label class="sliderLabel" for="checkSlider1">＞</label>
      </div>
    </div> 
  </div>
</template>

<script>

</script>

<style lang="scss" scoped>
@import '../assets/style/global/_color';
@import '../assets/style/global/_border';
@import '../assets/style/global/_sectionDefault';

.slider__contents{
  width: 70vw;
  height: calc(70vw * 1.61);
  margin: 0 auto;
  overflow: hidden;
  position: relative;
  &__content{
    min-width: 100%;
    position: absolute;
    top: 0;
    left: 0;
    transform: translateX(100%);
    &:nth-child(1) {
      animation: sliderAnime 6s ease-in-out infinite;
      z-index: 6;
    }
    &:nth-child(2) {
      animation: sliderAnime2 6s ease-in-out 1s infinite;
      z-index: -1;
    }
    &:nth-child(3) {
      animation: sliderAnime2 6s ease-in-out 3s infinite;
      z-index: -1;
    }
  }
}
 
@keyframes sliderAnime{
    0%{
        z-index: 5;
        transform: translateX(0);
    }
    16.6%{
        transform: translateX(0);
    }
    33.3%{
        transform: translateX(-100%);
    }
    50%{
        z-index: -1;
        transform: translateX(-100%);
    }
    66.6%{
        transform: translateX(100%);
    }
    83.2%{
        z-index: 5;
        transform: translateX(100%);
    }
    100%{
        z-index: 5;
        transform: translateX(0);
    }
}
 
@keyframes sliderAnime2{
    0%{
        z-index: 5;
        transform: translateX(100%);
    }
    16.6%{
        transform: translateX(0);
    }
    33.3%{
        transform: translateX(0);
    }
    50%{
        transform: translateX(-100%);
    }
    66.6%{
        z-index: -1;
        transform: translateX(-100%);
    }
    83.2%{
        transform: translateX(100%);
    }
    100%{
        z-index: 5;
        transform: translateX(100%);
    }
}

</style>