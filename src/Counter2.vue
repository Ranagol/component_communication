<template>
  <div>
    <p>Counter2.vue</p>
    <p>Counter: {{ counter }}</p>
    <button @click="decrease" class="btn btn-danger">Decrease</button>
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
        decrease(){
          this.counter --;
        }
      }
    }
</script>

<style>
    
</style>
