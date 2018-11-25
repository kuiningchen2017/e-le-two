<template>
  <div id="app">
    <ele-header></ele-header>
    <div id="list">
      <div class="list-item">
        <router-link to="/goods">goods</router-link>
      </div>
      <div class="list-item">
        <router-link to="/ratings">ratings</router-link>
      </div>
      <div class="list-item">
        <router-link to="/seller">seller</router-link>
      </div>
    </div>
    <router-view></router-view>
  </div>
</template>

<script>
import header from './components/header/header.vue'
export default {
  name: 'App',
  components: {
    'ele-header': header
  }
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
#list
  display flex
  .list-item
    width 0
    flex 1
    text-align center
    &:hover
      background-color yellowgreen
    a
      color: red
</style>
