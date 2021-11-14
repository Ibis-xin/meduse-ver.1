<template>
  <b-row class="ice">
    <b-col v-for="item in items" :key="item.index">
      <img :src="require(`@/assets/img/${item.src}.gif`)" :alt="item.alt"
    /></b-col>
    <b-row class="slogan">
      <b-col> Do&ensp; You&ensp; Want&ensp; Some&ensp; Dessert&ensp; ? </b-col>
    </b-row>
  </b-row>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { src: "ice-mango", alt: "芒果刨冰" },
        { src: "ice-matcha", alt: "抹茶刨冰" },
        { src: "ice-strawberry", alt: "草莓刨冰" },
        { src: "ice-milktea", alt: "奶茶刨冰" },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "../set/page.scss";
@import "../set/font.scss";
@import "../set/color.scss";

.ice {
  padding: $padding-secondary;
  img {
    padding: $padding-third;
    height: 3em;
  }
  .slogan {
    margin: $margin-main;
    font-family: $font-title;
    font-weight: $font-weight-text;
    color: $color-font;
  }
}
</style>