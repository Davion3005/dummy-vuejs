<template>
    <div class="list-user">
      <User v-for="user in listUser" v-bind:key="user.id" v-bind:user="user"></User>
    </div>
</template>

<script>
import User from './User'

export default {
  name: 'ListUser',
  components: {
    User
  },
  props: {
    listUser: {
      type: Array,
      default () {
        return []
      }
    }
  },
  data () {
    return {
      msg: 'List Users'
    }
  }
}
</script>

<style scoped>
  .list-user {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }
  .list-user .user {
    padding: 30px;
    margin-bottom: 30px;
    border: 2px solid #333;
    width: calc(33.3333% - 20px)
  }
</style>
