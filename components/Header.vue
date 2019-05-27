<template>
  <section class="header">
    <logo/>
    <nuxt-link class="link" to="/">Home</nuxt-link>
    <nuxt-link class="link" to="/about">About</nuxt-link>
    <nuxt-link class="link" to="/products">Products</nuxt-link>
    <nuxt-link class="link" to="/productCard">prodCard</nuxt-link>
  </section>
</template>

<script>
import Logo from './Logo'
  export default {
    name: "HeaderGosp",
    components: {
      Logo
    }
  }
</script>

<style lang="scss" scoped>
.header {
  box-sizing: border-box;
  width: 100%;
  height: 15vh;
  padding: 0 20px;
  background-image: url("../static/images/header_cloud.png");
  background-size: 100% 140%; 
  background-repeat: no-repeat; 
  .link {
    text-decoration: none;
    color: rgba(0,0,0,0.65);
    font-family: sans-serif;
    font-size: 1.7rem;
    height: 5vh;
    line-height: 15vh;
    margin: 0 7px;
    transition: .3s;
    color: green;
    text-shadow: 1px 2px 2px white;
    float:right;
    &:hover {
      color: black;
      text-shadow: 1px 2px 2px white;
    }
    &:after {
      display: block;
      content: "";
      clear: both;
    }
  }
}
</style>
