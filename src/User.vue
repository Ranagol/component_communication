<template>
    <div>
      <p>User.vue</p>
      <p>Name: {{ name }}</p>
      <p>Age: {{ age }}</p>
      <button @click="changeToMerlin" class="btn btn-info">Change name to Merlin</button>
      <button @click="changeToArthur" class="btn btn-info">Change name to Arthur</button>
      <hr>
      <userdetail-tag></userdetail-tag>
      <useredit-tag></useredit-tag>
    </div>
</template>

<script>
  import UserDetail from './UserDetail.vue';
  import UserEdit from './UserEdit.vue';
  
  export default {

    data: function(){
      return {
        name: 'Arthur',
        age: 29,
      }
    },

    methods: {
      changeToMerlin(){
        this.name = 'Merlin';
      },

      changeToArthur(){
        this.name = 'Arthur';
      }
    },

    components: {
      'useredit-tag': UserEdit,
      'userdetail-tag': UserDetail,
    }
  }
</script>

<style>
    
</style>