<template>
  <div>
    <p class="hoge">トップページ</p>
    <searchArea/>
   </div>
</template>

<script>
import searchArea from "@/components/searchArea";
export default {
  name: 'app',
  components: {
    searchArea,
  },
}
</script>

<style lang="scss">
@import './assets/style/global/_reset';
@import './assets/style/global/_common';
.sectionTitle {
  color: white;
  background-color: blue;
}
</style>
