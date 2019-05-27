<template>
  <nav class="left-sidebar">
    <ul class="categories">
      <li class="category" @click="openCategory">Хавчік
        <ul>
          <nuxt-link to="/products/vegetables" class="sub-category">Овочі</nuxt-link>
          <nuxt-link to="/products/fruits" class="sub-category">Фрукти</nuxt-link>
          <nuxt-link to="/products/meat" class="sub-category">Мясо</nuxt-link>
        </ul>
      </li>
      <li class="category" @click="openCategory">Огород
        <ul>
          <nuxt-link to="/products/seed" class="sub-category">Сємєна</nuxt-link>
          <nuxt-link to="/products/tools" class="sub-category">Інструмєнти</nuxt-link>
          <nuxt-link to="/products/fertilization" class="sub-category">Удобрєнія</nuxt-link>
        </ul>
      </li>
      <li class="category" @click="openCategory">Спєцовкі
        <ul>
          <nuxt-link to="/products/vacuum-cleaners" class="sub-category">Для рабатяг</nuxt-link>
          <nuxt-link to="/products/refrigerators" class="sub-category">Для брігадіра</nuxt-link>
          <nuxt-link to="/products/tiles" class="sub-category">Плитки</nuxt-link>
        </ul>
      </li>
    </ul>
  </nav>
</template>

<script>
  export default {
    name: "LeftSidebar",
    methods: {
      openCategory (event) {
        event.target.classList.toggle('active')
      }
    }
  }
</script>

<style lang="scss" scoped>
  .left-sidebar {
    width: fit-content;
    align-self: flex-start;
    background-color: rgba(0,0,0,0.41);
    border-top-right-radius: 20px;
    border-bottom-right-radius: 20px;
    padding: 10px 0;
    overflow: hidden;
    color: white;
    .categories {
      padding: 0;
      list-style: none;
      .category {
        font-size: 1.3rem;
        cursor: pointer;
        &.active {
          ul {
            height: 150px;
          }
        }
        ul {
          height: 0;
          padding: 0;
          display: flex;
          box-shadow: inset 0 0 10px 0 rgba(0,0,0,0.4);
          background-color: rgba(160,160,160,1);
          flex-direction: column;
          transition: .3s;
          overflow: hidden;
          a {
            box-shadow: inset;
            font-size: 1rem;
            padding: 5px 10px;
            text-decoration: none;
            color: white;
            text-align: left;
            transition: .3s;
            &:hover {
              padding-left: 20px;
            }
          }
        }
      }
    }
  }
</style>
