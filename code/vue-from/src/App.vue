<template>
  <form v-on:submit.prevent="submitFrom"> <!-- .prevent 아래 event.preventDefault();와 동일 이동이나 새로고침 막아줌 -->
    <div>
      <label for="username">id: </label> <!-- 데이터 연결 -->
      <input id="username" type="text" v-model="username">
    </div>
    <div>
      <label for="password">pw: </label>
      <input id="password" type="password" v-bind="password"> <!-- 데이터 연결 -->
    </div>
    <button type="submit">login</button> <!-- Login 버튼 -->
  </form>
</template>

<script>
import axios from 'axios'; // 브라우저에서 서버로 데이터를 주고 받기 위한 라이브러리

export default {
  data: function() {
    return {
      username: '',
      password: '',
    }
  },
  methods: {
    submitFrom: function() {
      // event.preventDefault(); //From 이동이나 새로고침을 막음
      console.log(this.username, this.password);
      var url = 'https://jsonplaceholder.typicode.com/users';
      var data = {
        username: this.username,
        password: this.password
      }
      axios.post(url, data) //포스트는 데이터를 생성하거나 저장할때 사용하는 메서드
        .then(function(response){
          console.log(response);
        })
        .catch(function(error) {
          console.log(error);
        });
    }
  }
}
</script>

<style>

</style>