<template>
  <div id="app" class="container">
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
