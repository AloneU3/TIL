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

#### 대신 그만큼 중복이 많을 수 있으니 데이터 같은 값을 function으로 넣음

<script>

export default {

  data: function() {

    return {

      str: 'hi'

    }

  }

  /*new Vue({

    data; {

      str: 'hi'

    }

  })위랑 동일*/

}

</script>

### 컴포넌트 이름은 최소한 두 단어로 조합해서 만듬

- HTML 표준 태그인지 뷰 컴포넌트 태그인지 브라우저가 구별할 수 있게 두 단어 이상을 조합해서 만듬
