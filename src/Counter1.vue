<template>
  <div>
    <p>Counter1.vue</p>
    <p>Counter: {{ counter }}</p>
    <button @click="increase" class="btn btn-danger">Increase</button>
  </div>


    
</template>

<script>
    export default {
      data: function(){
        return{
          counter:0,
        };
      },

      methods: {
        increase(){
          this.counter ++;
        }
      }
    }
</script>

<style>
    
</style>
