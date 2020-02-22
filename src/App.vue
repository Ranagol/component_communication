<template>
  <div id="app">
    <p>App.vue</p>
    <user-tag></user-tag>
    
  </div>
</template>

<script>
import User from './User.vue';
export default {
  name: 'app',
  data () {
    return {
      
    }
  },

  components: {
    'user-tag': User,
  }
}
</script>

<style>

</style>
