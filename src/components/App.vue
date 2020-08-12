<template>
  <div class="container">
    <div id="app">
      <BaseHeader></BaseHeader>
      <ListUser v-bind:listUser="users"></ListUser>
      <BaseFooter></BaseFooter>
    </div>
  </div>
</template>

<script>
import BaseHeader from './BaseHeader.vue'
import BaseFooter from './BaseFooter'
import ListUser from './ListUser'

export default {
  name: 'App',
  components: {
    BaseHeader,
    BaseFooter,
    ListUser
  },
  data () {
    return {
      title: 'The title from parent component',
      users: [
        {
          id: 1,
          name: 'Nguyen Cong Danh',
          email: 'DanhNC@gmail.com'
        },
        {
          id: 2,
          name: 'Tran Van Hung',
          email: 'HungTV@gmail.com'
        },
        {
          id: 3,
          name: 'Nguyen Luong Kim Phung',
          email: 'PhungNKL@gmail.com'
        },
        {
          id: 4,
          name: 'Tran Van A',
          email: 'AnhNC@gmail.com'
        },
        {
          id: 5,
          name: 'Nguyen Thi B',
          email: 'BaoCC@gmail.com'
        },
        {
          id: 6,
          name: 'Do Van C',
          email: 'CongAB@gmail.com'
        }
      ]
    }
  }
}
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
  .container {
    max-width: 1170px;
    margin: auto;
    padding: 15px;
  }
</style>
