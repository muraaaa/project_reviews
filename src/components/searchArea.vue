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
            <a href=# class="wordlist__item__link">Java</a>
            <a href=# class="wordlist__item__link">PHP</a>
            <a href=# class="wordlist__item__link">Python</a>
            <a href=# class="wordlist__item__link">JavaScript</a>
            <a href=# class="wordlist__item__link">フロントエンド</a>
            <a href=# class="wordlist__item__link">インフラ</a>
            <a href=# class="wordlist__item__link">Ruby</a>
            <a href=# class="wordlist__item__link">HTML5</a>
            <a href=# class="wordlist__item__link">月80万円以上</a>
            <a href=# class="wordlist__item__link">大阪</a>
            <a href=# class="wordlist__item__link">福岡</a>
            <a href=# class="wordlist__item__link">サーバー</a>
            <a href=# class="wordlist__item__link">Andorid</a>
            <a href=# class="wordlist__item__link">c#</a>
            <a href=# class="wordlist__item__link">プログラマー</a>
            <a href=# class="wordlist__item__link">SQL</a>
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
      background: no-repeat;
      background-color: $main;
      background-image: url(../assets/style/loupe.svg);
      background-position: center;
      background-size: 70%;
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
}

.hoge {
  color: red;
}
</style>