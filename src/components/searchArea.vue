<template>
  <section class="searchArea">
    <p class="contentTtl contentTtl__search" >案件を探す</p>
    <form action="#" id="ProjectSearchIndexForm">
      <div class="freeword">
        <ul class="freeword__info">
          <li class="freeword__info__text">
            案件数 <span class="highlight">7929</span> 件
          </li>
          <li class="freeword__info__text">
            <span>2019/09/25</span>更新
          </li>
        </ul>
        <div class="freeword__search">
          <input type="text" class="freeword__search__input" placeholder="例) Java 渋谷">
          <input type="submit" class="freeword__search__submitBtn" value>
        </div>
      </div>
    </form>
    <div class="recommendedWords">
      <p class="recommendedWords__ttl">オススメワード</p>
      <div class="recommendedWords__scrollArea">
        <ul class="wordlist">
          <li class="wordlist__item">
            <a href=# class="wordlist__item__link wordlist__item__link--code">Java</a>
          </li>
          <li class="wordlist__item">
            <a href=# class="wordlist__item__link wordlist__item__link--code">PHP</a>
          </li>
          <li class="wordlist__item">
            <a href=# class="wordlist__item__link wordlist__item__link--code">Python</a>
          </li>
          <li class="wordlist__item">
            <a href=# class="wordlist__item__link wordlist__item__link--code">JavaScript</a>
          </li>
          <li class="wordlist__item">
            <a href=# class="wordlist__item__link wordlist__item__link--laptop">フロントエンド</a>
          </li>
          <li class="wordlist__item">
            <a href=# class="wordlist__item__link wordlist__item__link--employee">インフラ</a>
          </li>
          <li class="wordlist__item">
            <a href=# class="wordlist__item__link wordlist__item__link--code">Ruby</a>
          </li>
          <li class="wordlist__item">
            <a href=# class="wordlist__item__link wordlist__item__link--code">HTML5</a>
          </li>
          <li class="wordlist__item">
            <a href=# class="wordlist__item__link wordlist__item__link--yenMark">月80万円以上</a>
          </li>
          <li class="wordlist__item">
            <a href=# class="wordlist__item__link wordlist__item__link--mapPointer">大阪</a>
          </li>
          <li class="wordlist__item">
            <a href=# class="wordlist__item__link wordlist__item__link--mapPointer">福岡</a>
          </li>
          <li class="wordlist__item">
            <a href=# class="wordlist__item__link wordlist__item__link--server">サーバー</a>
          </li>
          <li class="wordlist__item">
            <a href=# class="wordlist__item__link wordlist__item__link--mobile">Andorid</a>
          </li>
          <li class="wordlist__item">
            <a href=# class="wordlist__item__link wordlist__item__link--code">c#</a>
          </li>
          <li class="wordlist__item">
            <a href=# class="wordlist__item__link wordlist__item__link--employee">プログラマー</a>
          </li>
          <li class="wordlist__item">
            <a href=# class="wordlist__item__link wordlist__item__link--code">SQL</a>
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script>
</script>

<style lang="scss" scoped>
@import '../assets/style/global/_color';
@import '../assets/style/global/_border';

.contentTtl__search::before {
  top: 7px;
  background-size: 12px;
} 

.freeword {
  padding: 12px 12px 24px;
  background-color: #fff;
  &__info {
    display: flex;
    justify-content: space-between;
    align-items: baseline;
    padding-bottom: 4px;
    font-size: 0.875rem;
    span {
      font-weight: bold;
    }
  }
  &__search {
    position: relative;
    &__input {
      width: 100%;
      height: 46px;
      padding: 0 12px;
      border: $main_border;
      border-radius: 4px;
      box-shadow: 0 0 6px $boxShadow;
      font-size: 0.875rem;
    }
    &__submitBtn {
      position: absolute; 
      top: 0;
      right: 0;
      width: 50px;
      height: 46px;
      padding: 0;
      margin: 0;
      border: none;
      border-left: $main_border;
      border-radius: 0 3px 3px 0;
      background: $main url(../assets/style/svgs/loupe.svg) 50% no-repeat;
      background-size: 30px;
    }
  }
}

.recommendedWords {
  padding-bottom: 20px;
  &__ttl {
    padding: 0 12px;
    font-size: 0.875rem;
  }
  &__scrollArea {
    overflow: auto;
  }
}

.wordlist {
  display: flex;
  flex-wrap: wrap;
  width: 750px;
  margin: 4px 8px;
  &__item {
    display: block;
    margin: 3px;
    &__link {
      position: relative;
      display: block;
      padding: 8px 10px 8px 30px;
      border-radius: 2px;
      color: $mainFont;
      font-size: 0.75rem;
      &--code {
        background: $background url(../assets/style/svgs/codeBlack.svg) 10px 50% no-repeat;
      }
      &--laptop {
        background: $background url(../assets/style/svgs/laptop.svg) 10px 50% no-repeat;
      }
      &--employee {
        background: $background url(../assets/style/svgs/employee.svg) 10px 50% no-repeat;
      }
      &--yenMark {
        background: $background url(../assets/style/svgs/yenMark.svg) 10px 50% no-repeat;
      }
      &--mapPointer {
        background: $background url(../assets/style/svgs/mapPointer.svg) 10px 50% no-repeat;
      }
      &--server {
        background: $background url(../assets/style/svgs/server.svg) 10px 50% no-repeat;
      }
      &--mobile {
        background: $background url(../assets/style/svgs/mobile.svg) 10px 50% no-repeat;
      }

    }
  }
}
</style>