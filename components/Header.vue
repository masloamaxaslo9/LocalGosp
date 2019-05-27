<template>
  <section class="header">
    <nuxt-link class="link" to="/">Home</nuxt-link>
    <nuxt-link class="link" to="/about">About</nuxt-link>
    <nuxt-link class="link" to="/products">Products</nuxt-link>
  </section>
</template>

<script>
  export default {
    name: "Header.vue"
  }
</script>

<style lang="scss" scoped>
.header {
  box-sizing: border-box;
  width: 100%;
  border-bottom: 1px solid rgba(0,0,0,0.3);
  height: 5vh;
  padding: 0 20px;
  .link {
    text-decoration: none;
    color: rgba(0,0,0,0.65);
    font-family: sans-serif;
    font-size: 1.3rem;
    height: 5vh;
    line-height: 4.6vh;
    margin: 0 7px;
    transition: .3s;
    &:hover {
      color: rgba(0,0,0,0.9);
    }
  }
}
</style>
