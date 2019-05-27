<template>
  <section class="container">
    <h1 class="title">Products</h1>
    <div class="products">
      <LeftSidebar />
      <div class="product">

      </div>
    </div>
  </section>
</template>

<script>
  import LeftSidebar from '@/components/LeftSidebar'

  export default {
    name: "index.vue",
    components: {
      LeftSidebar
    }
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
    .product {
      width: calc( 100% - 121px );
      padding: 0 15px;
      background-color: rgba(0,255,0,0.4);
      min-height: calc( 95vh - 75px );
    }
  }
</style>
