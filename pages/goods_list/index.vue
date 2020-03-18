<template>
  <div>
      <h2>这是商品列表</h2>
      <ul>
          <li :key="item.id" v-for="(item) in list">
              <nuxt-link :to="'/detail/'+item.id">{{item.name}}</nuxt-link>
            </li>
      </ul>
  </div>
</template>

<script>
export default {
  asyncData({app}) {
    // console.log(app)
    const arr = app.sort([1,2,4,5,2,7])
    console.log(arr)
    const arr2 = app.$integerSort([1,2,4,5,2,7]);
    console.log(arr2)
  },
  mounted() {
    const arr3 = this.$integerSort([1,2,4,5,2,7])
  },
  
  data() {
      return {
          list: [
              {id:1,name:'iphone', price: 2000},
              {id:2,name:'华为', price: 2001},
              {id:3, name:'小米', price: 2003},
          ]
      }
  }
}
</script>

<style lang="sass" scoped>
</style>
