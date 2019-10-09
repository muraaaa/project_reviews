<template>
  <section class="newProject">
    <p class="contentTtl contentTtl__new" >新着案件</p>
    <div class="projectCard__container">
      <a href="#" >
        <div class="projectCardDetail">
          <h3 class="projectCardDetail__ttl">
            <span class="projectCardDetail__ttl__label">New</span>
            <strong>【コーディング】自社クーポンサービスサイト制作</strong>のエンジニア求人・案件
          </h3>
          <div class="projectCardDetail__summary">
            <p class="projectCardDetail__summary__rewards">
              〜<span class="highlight projectCardDetail__summary__rewards-bold">60万</span>円/月
            </p>
            <p class="projectCardDetail__summary__category">
              業務委託
            </p>
          </div>
          <table class="projectCardTable">
            <tr class="projectCardTable__row">
              <th class="projectCardTable__row__head">最寄り駅</th>
              <td class="projectCardTable__row__body">肥後橋（大阪府）</td> 
            </tr>
            <tr class="projectCardTable__row">
              <th class="projectCardTable__row__head">開発環境</th>
              <td class="projectCardTable__row__body">
                <div class="projectCardTable__row__body__content">
                  AWS，PHP，SQL，JavaScript，HTML，ActionScript，CSS，Git
                </div>
              </td> 
            </tr>
          </table>
        </div>
      </a>
      <a href="#" >
        <div class="projectCardDetail">
          <h3 class="projectCardDetail__ttl">
            <span class="projectCardDetail__ttl__label">New</span>
            <strong>【UIデザイン】webブラウザゲームのUI,UXデザインの設計支援</strong>
            のエンジニア求人・案件
          </h3>
          <div class="projectCardDetail__summary">
            <p class="projectCardDetail__summary__rewards">
              〜<span class="highlight projectCardDetail__summary__rewards-bold">60万</span>円/月
            </p>
            <p class="projectCardDetail__summary__category">
              業務委託
            </p>
          </div>
          <table class="projectCardTable">
            <tr class="projectCardTable__row">
              <th class="projectCardTable__row__head">最寄り駅</th>
              <td class="projectCardTable__row__body">六本木（東京都）</td> 
            </tr>
          </table>
        </div>
      </a>
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

.contentTtl__new {
  margin-bottom: 16px;
  &::before {
    background-image: url(../assets/style/pngs/icoTopMenu_new.png);
  }
}

.projectCardDetail {
  margin: 16px 12px 0;
  padding: 12px 12px 16px;
  border: $main_border;
  border-radius: 4px;
  box-shadow: 0 1px 2px rgba(0, 0, 0, .16);
  &__ttl {
    font-size: 0.875rem;    
    font-weight: bold;
    color: #333;
    &__label {
      padding: 4px 6px;
      font-size: 0.75rem;
      color: $newProject;
      border: 1px solid $newProject;
    }
    strong {
      font-size: 1rem;
      color: $main;
    }
  }
  &__summary {
    display: flex;
    margin: 16px 0 8px;
    justify-content: flex-start;
    align-items: baseline;
    font-size: 0.875rem;
    color: #333;
    &__rewards {
      padding: 0 0 0 22px;
      margin: 0 16px 0 0;
      background: url(../assets/style/svgs/salary.svg) left center no-repeat;
      background-size: 18px;
      &-bold {
        font-weight: bold;
      }
    }
    &__category {
      padding: 0 0 0 22px;
      background: url(../assets/style/svgs/category.svg) left center no-repeat;
      background-size: 18px;
    }
  }
}

.projectCardTable {
  width: 100%;
  border: $main_border;
  table-layout: fixed;
  font-size: 0.875rem;
  color: #333;
  &__row {
    border-bottom: $main_border;
    &__head {
      width: 91px;
      padding: 4px 8px;
      background-color: $tableHead;
      vertical-align: middle;
      text-align: left;
    }
    &__body {
      width: 100%;
      padding: 4px 8px;
      &__content {
        overflow: hidden;
        word-break: normal;
        white-space: nowrap;
        text-overflow: ellipsis;
      }
    }
  }
}

.newJobs {
  margin: 8px 0 20px;
  text-align: right;
  &__link {
    padding-left: 15px;
    margin-right: 10px;
    color: $main;
    font-weight: bold;
    font-size: 0.75rem;
    background: url(../assets/style/pngs/icnLink_transparent.png) left no-repeat; 
  }
}
</style>