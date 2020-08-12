<template>
  <p class="user">{{ user.name + ' ' + user.email}}</p>
</template>

<script>
export default {
  name: 'User',
  props: {
    user: {
      type: Object,
      default () {
        return {}
      }
    }
  },
  data () {
    return {
      msg: 'User'
    }
  }
}
</script>

<style scoped>

</style>
