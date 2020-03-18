<template>
    <div>
        <h2>Home page</h2>
        <button @click='sayHello()'>say hello</button>
    </div>
</template>
<script>


export default {
  methods: {
      sayHello() {
          this.$myInjectedFunction('say,hello!!')
      }
  }
}
</script>
<style lang="sass" scoped>

</style>

