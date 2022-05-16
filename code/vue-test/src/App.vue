<template>
  <form v-on:submit.prevent>
    <div>
      <label for="userid">id: </label>
      <input id="userid" type="text" v-model="userid">
    </div>
    <div>
      <label for="password">pw: </label>
      <input id="password" type="text" v-model="password">
    </div>
      <button>login</button>
  </form>
</template>

<script>
export default {
  data: function(){
    return {
       userid: '',
       password: ''
    }
  }
}
</script>

<style>

</style>