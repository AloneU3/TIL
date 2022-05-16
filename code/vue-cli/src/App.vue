<template>
    <div>
      <app-header
       v-bind:propsdata="str" 
       v-on:renew="renewStr">
      </app-header>
    </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'; //AppHeader에 있는 내용을 변수에 담는다

//var AppHeader = {
//  template: '<header><h1>Header</h1></header>'
//}

export default {
  data: function() {
    return {
      str: 'Header' //디폴트론 Header가 출력
    }
  },
  components: {
    'app-header': AppHeader //해당 변수를 연결
  },
  methods: {
    renewStr: function() {
      this.str = 'hi'; //버튼을 클릭시 Header가 hi로 바뀜
    }
  }
  /*new Vue({
    data; {
      str: 'hi'
    }
  })위랑 동일*/
}
</script>

<style>

</style>