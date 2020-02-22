<template>
<div>
  <p>UserEdit.vue edits the age</p>
  <p>Ageuseredit: {{ age }}</p>
</div>
    
</template>

<script>

  import { eventBus } from './main';
    export default {
      props: ['age'],

    }
</script>

<style>
    
</style>