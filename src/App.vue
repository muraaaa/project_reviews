<template>
  <div>
    <searchArea/>
   </div>
</template>

<script>
import searchArea from "@/components/searchArea";
/* import searchArea from "@/components/searchArea";*/
export default {
  name: 'app',
  components: {
    searchArea,
    /* serchArea,*/
  },
}
</script>

<style lang="scss">
@import './assets/style/global/_reset';
@import './assets/style/global/_common';

.contentTtl {
  padding: 5px 0 5px 32px;
  font-size: 0.875rem;
  font-weight: bold;
  color: #fff;
  background-color: #37789b;
}
</style>
