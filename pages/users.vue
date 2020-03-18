<template>
  <div>
    <h2>这是users组件</h2>
    <nuxt-link to="/users/">嵌套首页</nuxt-link>
    <nuxt-link to="/users/profile">嵌套详情</nuxt-link>
    <nuxt/>
  </div>
</template>

<script>
export default {
  data() {
    return {

    }
  },
  created(){

  },
  methods: {

  }
}
</script>

<style lang="less" scoped>
</style>
