# 싱글 파일 컴포넌트(.vue)

- HTML, CSS, Javascript를 한 파일에 관리할 수 있다

- var appHeader = {
  
      template: '<dev>header</dev>',
  
      methods: {
  
          addNum: function() {
  
          }
  
      }
  
  }
  
  <template>
  
      <div>appHeader</div>
  
      <!-- HTML -->
  
  </template>
  
  <script>
  
  export default {
  
      //자바스크립트 - 인스턴스 옵션
  
          methods: {
  
          addNum: function() {
  
          }
  
      }
  
  }
  
  </script>
  
  <style>
  
      /*CSS*/
  
  </style>

위 같은 느낌으로 가능
