<template>
  <section class="newProject">
    <p class="contentTtl contentTtl__new" >新着案件</p>
    <div class="projectCard__container">
      <a href="#" >
        <div class="projectCardDetail">
          <h3 class="projectCardDetail__ttl">
            <span class="projectCardDetail__ttl__label">New</span>
            <strong>【コーディング】自社クーポンサービスサイト制作</strong>
          </h3>
          <div class="projectCardDetail__summary">
            <p class="projectCardDetail__summary__rewards">
              〜<span class="highlight">60万</span>円/月
            </p>
            <p class="projectCardDetail__categoty">
              業務委託
            </p>
            <table class="projectCardTable">
              <tr class="projectCardTable__row">
                <th class="projectCardTable__row__head">最寄駅</th>
                <tb class="projectCardTable__row__body">六本木（東京都）</tb> 
              </tr>
            </table>
          </div>
        </div>
      </a>
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
}

.projectCardDetail {
  margin: 0 12px;
  padding: 12px 12px 16px;
  border: $main_border;
  border-radius: 4px;
  color: $mainFont;
}

</style>