<template>
  <section class="container">
    <h1 class="title">Products</h1>
    <div class="products">
      <nav class="left-sidebar">
        <ul class="categories">
          <li class="category">Електроніка
            <ul>
              <nuxt-link to="/products/laptops" class="sub-category">Ноутбуки</nuxt-link>
              <nuxt-link to="/products/smart-phones" class="sub-category">Смартфони</nuxt-link>
              <nuxt-link to="/products/televisions" class="sub-category">Телевізори</nuxt-link>
            </ul>
          </li>
          <li class="category">Інструменти
            <ul>
              <nuxt-link to="/products/bulgarians" class="sub-category">Болгарки</nuxt-link>
              <nuxt-link to="/products/screwdriver" class="sub-category">Шуруповерт</nuxt-link>
            </ul>
          </li>
          <li class="category">Побутова техніка
            <ul>
              <nuxt-link to="/products/vacuum-cleaners" class="sub-category">Пилососи</nuxt-link>
              <nuxt-link to="/products/refrigerators" class="sub-category">Холодильники</nuxt-link>
              <nuxt-link to="/products/tiles" class="sub-category">Плитки</nuxt-link>
            </ul>
          </li>
        </ul>
      </nav>
      <div class="product">

      </div>
    </div>
  </section>
</template>

<script>
  export default {
    name: "index.vue"
  }
</script>

<style lang="scss" scoped>
  .container {
    font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    margin: 0 auto;
    min-height: 95vh;
    display: flex;
    justify-content: flex-start;
    text-align: center;
    align-items: normal;
    flex-direction: column;
  }
  .title {
    color: #35495e;
    letter-spacing: 1px;
    margin: 15px;
  }
  .products {
    display: flex;
    justify-content: space-between;
    align-items: center;
    .left-sidebar {
      width: fit-content;
      align-self: flex-start;
      .categories {
        padding: 0;
        list-style: none;
      }

    }
    .product {
      width: 75%;
      background-color: green;
      min-height: calc( 95vh - 75px );
    }
  }
</style>
