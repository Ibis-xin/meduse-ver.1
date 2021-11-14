<template>
  <!-- <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view/>
  </div> -->
  <b-container fluid>
    <b-row class="header"></b-row>
    <b-row class="main">
      <b-col class="left"></b-col>
      <b-col cols="8" class="center">
        <b-row class="index">
          <b-col class="lead">
            <ice-list></ice-list>
          </b-col>
        </b-row>
        <b-row class="home">
          <introduction></introduction>
        </b-row>
        <b-row class="about">
          <img class="rounded mx-auto feature" src="./assets/img/sundae.gif" alt="聖代" />
        </b-row>
        <b-row class="more">
          <h2 class="menu">menu</h2>
          <br />
          <dessert-list></dessert-list>
        </b-row>
        <b-row class="source">
          <h2 class="author">chef</h2>
          <a href="https://www.plurk.com/1515dd"> Los </a>
        </b-row>
      </b-col>
      <b-col class="right"></b-col>
    </b-row>
    <b-row fluid class="footer"></b-row>
  </b-container>
</template>

<style lang="scss">
@import "@/style/style.scss";
</style>

<script>
import IceList from "./components/IceList.vue";
import Introduction from "./components/Introduction.vue";
import DessertList from "./components/DessertList.vue";
export default {
  components: {
    IceList,
    Introduction,
    DessertList,
  },
};
</script>
