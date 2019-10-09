<template>
  <div>
    <searchArea/>
    <newProject/>
   </div>
</template>

<script>
import searchArea from "@/components/searchArea";
import newProject from "@/components/newProject";
/* import searchArea from "@/components/searchArea";*/
export default {
  name: 'app',
  components: {
    searchArea,
    newProject,
    /* serchArea,*/
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
