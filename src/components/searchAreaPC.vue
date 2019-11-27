<template>
  <section class="searchArea">
    <section class="contentTtlPcWithPic">
      <img src="../assets/style/svgs/search.svg" class="contentTtlPcWithPic__pic">
      <p class="contentTtlPcWithPic__main">案件を探す</p>
      <p class="contentTtlPcWithPic__sub">Search</p>
    </section>
    <section class="search">
      <form action="#" id="ProjectSearchIndexFormPc">
        <div class="freewordPc">
          <div class="freewordPc__info">
            <p class="freewordPc__info__text">
              該当件数：<span class="highlight">7929</span> 件
            </p>
          </div>
          <div class="freewordPc__search">
            <input type="text" class="freewordPc__search__input" placeholder="職種、ツール、仕事内容など">
            <div class="searchBar">
              <input type="text" id="label1" class="searchBar__language" placeholder="言語" readonly>
              <div class="searchBar__language--click pulldown">
                <div class="pulldown__header">
                  <p class="pulldown__header__ttl headerLanguage">
                    <span>言語</span>
                    を選択
                  </p>
                </div>
              </div>
              <input type="text" id="label2" class="searchBar__region" placeholder="エリア" readonly>
              <div class="searchBar__region--click pulldown">
                <div class="pulldown__header">
                  <p class="pulldown__header__ttl headerRegion">
                    <span>エリア</span>
                    を選択
                  </p>
                </div>
              </div>
            </div>
            <!-- <div class="searchBar">
              <input type="checkbox" id="label1" class="searchBar__input">
              <label for="label1" class="searchBar__language">language</label>
              <div class="searchBar__language--click pulldown">
                <div class="pulldown__header">
                  <p class="pulldown__header__language">
                    <span>言語</span>
                    を選択
                  </p>
                </div>
              </div>
              <input type="checkbox" id="label2" class="searchBar__input">
              <label for="label2" class="searchBar__region">region</label>
              <div class="searchBar__region--click">
                <p>bbb</p>
              </div>
            </div> -->
            <input type="submit" class="freewordPc__search__submitBtn" value>
          </div>
        </div>
      </form>
      <div class="recommendedWords">
        <p class="recommendedWords__ttl">オススメワード:</p>
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
  </section>
</template>

<script>
</script>

<style lang="scss" scoped>
@import '../assets/style/global/_color';
@import '../assets/style/global/_border';
@import '../assets/style/global/_sectionDefault';

// transition timeの設定を忘れない

.searchArea {
  @extend %sectionDefault;
}

%border {
  border: $main_border;
  border-radius: 4px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}
%borderHover {
  border-color: #b3b3b3;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}
%borderFocus {
  border: $main_border;
  border-radius: 4px;
  border-color: $main;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  outline: none;
}
.freewordPc {
  font-size: 0.875rem;
  &__info {
    margin-bottom: 14px;
    &__text {
      span {
        margin: 0 5px;
        font-size: 1.5rem;
        font-weight: bold;
      }
    }
  }
  &__search {
    display: flex;
    justify-content: space-between;
    margin-bottom: 30px;
    &__input {
      width: 300px;
      padding: 16px 14px;
      font-size: 0.875rem;
      @extend %border;
      &:hover {
        @extend %borderHover;
      }
      &:focus {
        @extend %borderFocus;
        // @extend %border;
        // @extend %borderHover;
        // border-color: $main;
        // outline: none;
      }
    }
    &__submitBtn {
      width: 110px;
      @extend %border;
      @extend %borderFocus;
      background: $main url(../assets/style/svgs/loupe.svg) 50% no-repeat;
      background-size: 40px;
    }
  }
}
.searchBar {
  position: relative;
  display: flex;
  flex-wrap: wrap;
  &__input {
    display: none;
  }
  &__language {
    position: relative;
    width: 186px;
    padding: 12px 28px 12px 40px;
    @extend %border;
    background: 6px 10px no-repeat;
    background-image: url(../assets/style/svgs/codeGray.svg);
    background-size: 25px;
    color: #999;
    font-size: 0.875rem;
    &::after {
      content: url(../assets/style/svgs/arrow.svg);
      position: absolute;
      top: 12px;
      right: 14px;
      display: block;
      width: 14px;
      &:active {
        transform: rotate(180deg);
      }
    }
    &:focus {
      @extend %borderFocus;
      background-image: url(../assets/style/svgs/codeMainColor.svg);
    }
    &:focus::placeholder,
    &:focus::before {
      color: #333;
    }
    &:focus ~ .searchBar__language--click {
      visibility: visible;
    }
    &:hover {
      @extend %borderHover;
      color: #333;
    }
    &--click {
      visibility: hidden;
      position: absolute;
      top: 70px;
      // sectionの頭に揃える　(900 - (300 + 404 + 110)) / 2
      left: -343px;
      width: 900px;
    }
  }
  &__region {
    @extend .searchBar__language;
    order: 2;
    &:hover {
      @extend %borderHover;
      color: #333;
    }
    &:focus {
      @extend %borderFocus;
    }
    &:focus ~ .searchBar__region--click {
      visibility: visible;
    }
    &--click {
      visibility: hidden;
      position: absolute;
      top: 70px;
      left: -343px;
      width: 900px;
    }
  }
  &::before {
    content: url(../assets/style/svgs/cross.svg);
    order: 1;
    align-self: center;
    margin: auto 8px;
  }
}

.pulldown {
  display: block;
  height: 100px;
  @extend %borderHover;
  z-index: 10;
  background-color: #ffffff;
  &__header {
    padding: 20px 0;
    margin: 0 16px;
    border-bottom: 1px solid #d9d9d9;
    color: $main;
    &__ttl {
      padding: 0 0 0 32px;
      span {
        font-size: 1.125rem;
      }
    }
    &__language {
      background: url();
      color: $main;
    }
  }
}

.headerLanguage {
  &::before {
    
  }
}

.recommendedWords {
  display: flex;
  margin: 20px 0;
  &__ttl {
    margin-top: 1px;
    font-size: 0.875rem;
    line-height: 28px;
  }
  &__scrollArea {
    max-width: 660px;
    margin-left: 5px;
    line-height: 28px;
  }
}

.wordlist {
  display: flex;
  flex-wrap: wrap;
  &__item {
    flex: 1 0 auto;
    margin: 0 3px 7px;
    border-radius: 4px;
    background-color: $background;
    text-align: center;
    &__link {
      padding: 0 15px;
      color: $mainFont;
      font-size: 0.875rem;
    }
  }
}


</style>
