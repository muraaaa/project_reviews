<template>
  <section>
    <p class="sectionTitle" >
      このコンポーネントはseachareaです
    </p>
    <img src="" >
    <li v-for="item in listItems">
      <a :class="'wordList__item__link--' + item.iconType">{{ item.name }}</a>
    </li>
  </section>
</template>

<script>
export default {
  data() {
    return {
      listItems: [
        { name: "Java", iconType: "code" },
        { name: "PHP", iconType: "code" },
        { name: "Python", iconType: "laptopCode" },
        { name: "JavaScript", iconType: "laptopCode" },
      ]
    }
  }
}
</script>
<style lang="scss" scoped>
.hoge {
  color: red;
}
</style>