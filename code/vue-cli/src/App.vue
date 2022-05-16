<template>
    <div>
      <app-header></app-header>
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
      str: 'hi'
    }
  },
  components: {
    'app-header': AppHeader //해당 변수를 연결
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