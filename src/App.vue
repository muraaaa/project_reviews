<template>
  <div>
    <!-- 読み込んだ時に呼び出すコンポーネントを区別している -->
    <template v-if="mediaSP">
      <searchArea />
      <newProject />
    </template>
    <template v-else>
      <searchAreaPC />
      <newProject />
      <searchProjectByCategory />
    </template>
   </div>
</template>

<script>
import searchArea from "@/components/searchArea";
import searchAreaPC from "@/components/searchAreaPC";
import newProject from "@/components/newProject";
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

.highlight {
  font-size: 1.25rem;
  color: $highlight;
}
</style>
