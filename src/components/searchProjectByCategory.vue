<template>
  <div class="searchTab">
    <div class="searchTab__list">
      <input type="radio" id="tab__lang" name="searchTab__list__item" checked>
      <label for="tab__lang" class="searchTab__list__item">言語で探す</label>
      <input type="radio" id="tab__infra" name="searchTab__list__item">
      <label for="tab__infra" class="searchTab__list__item">インフラで探す</label>
      <input type="radio" id="tab__category" name="searchTab__list__item">
      <label for="tab__category" class="searchTab__list__item">職種で探す</label>
      <input type="radio" id="tab__industry" name="searchTab__list__item">
      <label for="tab__industry" class="searchTab__list__item">業界で探す</label>
      <input type="radio" id="tab__area" name="searchTab__list__item">
      <label for="tab__area" class="searchTab__list__item">エリアで探す</label>
      <div class="searchTab__body tabBody__language">
        <ul class="searchLinkList">
          <li class="searchLinkList__item">
            <a href="#">Java</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">Java</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">Java</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">Java</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">Java</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
        </ul>
      </div>
      <div class="searchTab__body tabBody__infra">
        <ul class="searchLinkList">
          <li class="searchLinkList__item">
            <a href="#">Linux</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">Linux</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">Linux</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">Linux</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">Linux</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
        </ul>
      </div>
      <div class="searchTab__body tabBody__category">
        <ul class="searchLinkList">
          <li class="searchLinkList__item">
            <a href="#">アプリケーションエンジニア</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">アプリケーションエンジニア</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">アプリケーションエンジニア</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">アプリケーションエンジニア</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">アプリケーションエンジニア</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
        </ul>
      </div>
      <div class="searchTab__body tabBody__industry">
        <ul class="searchLinkList">
          <li class="searchLinkList__item">
            <a href="#">ソーシャルゲーム</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">ソーシャルゲーム</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">ソーシャルゲーム</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">ソーシャルゲーム</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">ソーシャルゲーム</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
        </ul>
      </div>
      <div class="searchTab__body tabBody__area">
        <ul class="searchLinkList">
          <li class="searchLinkList__item">
            <a href="#">東京都(23区内)</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">東京都(23区内)（）</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">東京都(23区内)()</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">東京都(23区内)</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
          <li class="searchLinkList__item">
            <a href="#">東京都(23区内)</a>
            <span class="searchLinkList__item__number">(1642件)</span>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>
<script>
// export default {

// }
</script>
<style lang="scss" scoped>
@import '../assets/style/global/_color';
@import '../assets/style/global/_border';
@import '../assets/style/global/_sectionDefault';

.searchTab {
  @extend %sectionDefault;
  min-height: 300px;
  padding-bottom: 20px;
  margin-bottom: 8px;
  border-bottom: 2px solid #3d5c6d;
  overflow: hidden;
  &__list {
    position: relative;
    justify-content: space-around;
    padding: 5px 0;
    &::after {
      position: absolute;
      top: 45px;
      content: '';
      display: block;
      width: 100%;
      height: 10px;
      border-bottom: 2px dashed #3d5c6d;
    }
    input[name="searchTab__list__item"] {
      display: none;
    }
    #tab__lang:checked ~ .tabBody__language,
    #tab__infra:checked ~ .tabBody__infra,
    #tab__category:checked ~ .tabBody__category,
    #tab__industry:checked ~ .tabBody__industry,
    #tab__area:checked ~ .tabBody__area {
      display: block;
      animation-name: fade-in;
      animation-duration: 0.5s;
      animation-timing-function: ease-in-out;
      @keyframes fade-in {
        0% {Opacity: 0; transform: translate3d(0, 20px, 0);}
        100% {Opacity: 1; transform: translate3d(0, 0, 0);}     
      }
    }
    input:checked + .searchTab__list__item {
      background-color: $main;
      color: #fff;
      font-weight: bold;
      transition: 0.3s ease-in-out;
    }
    &__item {
      float: left;
      width: (900px - 40px) / 5;
      border-radius: 4px;
      background-color: $background;
      line-height: 40px;
      font-size: 0.875rem;
      text-align: center;
      &:not(:first-of-type) {
        margin-left: 10px;
      }
      &:hover {
        background-color: #d5d5d5;
      }

    }
  }
  &__body {
    display: none;
    clear: both;
    overflow: hidden;
    min-height: 240px;
    padding: 16px;
  }
}

.searchLinkList {
  display: flex;
  flex-wrap: wrap;
  &__item {
    position: relative;
    width: 25%;
    padding: 5px 0 5px 15px;
    font-size: 0.875rem;
    line-height: 1.225rem;
    &::before {
      content: '';
      position: absolute;
      top: 12.5px;
      left: 0;
      display: block;
      width: 5px;
      height: 5px;
      border-top: 2px solid #999;
      border-right: 2px solid #999;
      transform: rotate(45deg);
    }
    &__number {
      padding-left: 5px;
      color: #999;
      font-size: 0.6875rem;
    }
  }
}
</style>
