<template>
  <div id="app" class="container">
    <p>App.vue</p>
    <div class="row">
      <button @click="selectedComponent='appUser'" class="btn btn-success">User</button>
      <button @click="selectedComponent='appCounter1'" class="btn btn-success">Counter1</button>
      <button @click="selectedComponent='appCounter2'" class="btn btn-success">Counter2</button>
    </div>
    <p>The selected component is: {{ selectedComponent }}</p>
    <keep-alive>
      <component :is="selectedComponent">

      </component>
    </keep-alive>
  </div>
</template>

<script>
import User from './User.vue';
import Counter1 from './Counter1.vue';
import Counter2 from './Counter2.vue';

export default {
  name: 'app',
  data () {
    return {
      selectedComponent: 'appUser',
    }
  },

  components: {
    'appUser': User,
    'appCounter1': Counter1,
    'appCounter2': Counter2,
  }
}
</script>

<style>

</style>
