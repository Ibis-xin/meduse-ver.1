<template>
  <b-col class="introduction">
    <h1 class="title">
      <hr />
      Méduse
      <hr />
    </h1>
    Le dessert est le dernier plat sucré d'un repas occidental, ou on peut dire
    qu'il s'agit d'un aliment sucré que les Occidentaux mangent après un repas.
    <br />
    Il peut s'agir d'un plateau de fruits, de petits gâteaux, de tartes, de
    pudding ou de crème glacée. <br />
    De nos jours, le mot dessert en chinois peut également désigner tous les
    aliments sucrés . <br /><br />
    <b-col class="line">
      <img
        v-for="item in 3"
        :key="item"
        src="../assets/img/donut.gif"
        alt="甜甜圈"
      />
    </b-col>
    <br />
    Des solides et des liquides peuvent être inclus.Par exemple, l'eau sucrée et
    la soupe sucrée sont également des desserts et peuvent être considérées
    comme des collations.
  </b-col>
</template>

<script>
export default {};
</script>

<style lang="scss">
@import "../set/page.scss";
@import "../set/font.scss";
@import "../set/color.scss";

.introduction {
  padding: $padding-third;
  font-family: $font-text;
  font-weight: $font-weight-text;
  color: $color-font;
  line-height: 3em;
  .title {
    padding: $padding-third;
    font-family: $font-title;
    font-weight: $font-weight-title;
    color: $color-font;
  }
  img {
    margin: 0em 1em;
    line-height: 0em;
    height: 1em;
  }
}
</style>