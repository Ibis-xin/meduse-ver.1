<template>
  <ul class="dessert">
    <li v-for="item in items" :key="item.index">
      <img :src="require(`@/assets/img/${item.src}.gif`)" :alt="item.alt" />{{
        item.value
      }}
    </li>
  </ul>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { src: "muffin", alt: "鬆餅", value: 230 },
        { src: "pineapple", alt: "菠蘿麵包", value: 80 },
        { src: "croissant", alt: "可頌", value: 100 },
        { src: "cake", alt: "蛋糕", value: 160 },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "../set/page.scss";
@import "../set/font.scss";
@import "../set/color.scss";

.dessert {
  padding: $padding-secondary;
  width: 80%;
  *{
    text-align: left;
    height: 5em;
    font-family: $font-text;
    font-weight: $font-weight-text;
    color: $color-font;
  }
}
</style>