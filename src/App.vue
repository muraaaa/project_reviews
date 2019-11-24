<template>
  <div>
    <!-- 読み込んだ時に呼び出すコンポーネントを区別している -->
    <template v-if="mediaSP">
      <searchArea />
      <newProject />
    </template>
    <template v-else>
      <searchAreaPC />
      <searchProjectByCategory/>
      <newProjectPC />
    </template>
   </div>
</template>

<script>
import searchArea from "@/components/searchArea";
import searchAreaPC from "@/components/searchAreaPC";
import newProject from "@/components/newProject";
import newProjectPC from "@/components/newProjectPC";
import searchProjectByCategory from "@/components/searchProjectByCategory";
export default {
  name: 'app',
  data() {
    return {
      // 読み込んだ時にSP幅かどうかの判定
      mediaSP: window.innerWidth <= 480,
    }
  },
  components: {
    searchArea,
    searchAreaPC,
    newProject,
    newProjectPC,
    searchProjectByCategory
  },
}
</script>

<style lang="scss">
@import './assets/style/global/_reset';
@import './assets/style/global/_common';
@import './assets/style/global/_color';
@import './assets/style/global/_border';


.contentTtl {
  position: relative;
  padding: 5px 0 5px 32px;
  font-size: 0.875rem;
  font-weight: bold;
  color: #fff;
  background-color: $main;
  &::before {
    content: '';
    display: inline-block;
    position: absolute;
    top: 5px;
    left: 12px;
    width: 20px;
    height: 20px;
    background: url(./assets/style/pngs/icoSearch.png) left center no-repeat;
    background-size: 14px;
  }
}

.contentTtlPcWithPic {
  padding: 10px 0;
  margin: 20px auto;
  text-align: center;
  &__pic {
    width: 25px;
    height: 25px;
  }
  &__main {
    font-size: 1.75rem;
  }
  &__sub {
    color: $main;
    font-size: 0.625rem;
    font-weight: bold;
  }
}

.contentTtlPcWithoutPic {
  position: relative;
  padding-left: 20px;
  margin: 10px 0;
  line-height: 1.3;
  &::before {
    position: absolute;
    top: 0;
    left: 0;
    content: '';
    display: block;
    width: 6px;
    height: 100%;
    background-color: $main;
  }
  &::after {
    @extend .contentTtlPcWithoutPic::before;
    height: 30%;
    background-color: #ccc;
  }
  &__sub {
    color: $main;
    font-size: 0.625rem;
  }
  &__main{ 
    font-size: 1.25rem;
  }
}


.highlight {
  font-size: 1.25rem;
  color: $highlight;
}

</style>
