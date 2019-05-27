<template>
  <section class="container">
    <h1 class="title">
      Сторінка <b>{{ urlPage.id | capitalize}}</b>
    </h1>
  </section>
</template>

<script>
  export default {
    name: "_id",
    data() {
      return {
        urlPage: this.$route.params
      }
    },
    filters: {
      capitalize: function (value) {
        if (!value) return '';
        value = value.toString();
        return value.charAt(0).toUpperCase() + value.slice(1)
      }
    }
  }
</script>

<style scoped>

</style>
