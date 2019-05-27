<template>
  <div class="card">
    <left-sidebar></left-sidebar>
    <h1 class="card_title">title</h1>
    <img class="card_img" src="" alt="">
    <p class="card_description">description</p>
    <p class="card_price">price</p>
    <p class="card_category">category</p>
    <button class="card_btn">в корзинку</button>
  </div>
</template>

<script>
import leftSidebar from "../../components/LeftSidebar.vue"
export default {
  components: {
    leftSidebar
  }
}
</script>

<style>

</style>
