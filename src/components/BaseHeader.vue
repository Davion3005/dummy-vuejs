<template>
  <header><h1>{{ headerTitle }}</h1></header>
</template>

<script>
export default {
  name: 'BaseHeader',
  data () {
    return {
      msg: 'HEADER'
    }
  },
  props: {
    headerTitle: {
      type: String,
      default: 'No Title'
    }
  }
}
</script>

<style scoped>

</style>
