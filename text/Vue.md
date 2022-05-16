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



## 싱글 컴포넌트 (.Vue) 파일간에 데이터 공유

- import AppHeader from './components/AppHeader.vue'
  
  임포트 이름 URL로 다른 싱글 컴포넌트에 데이터를 받아올 수 있다

- props랑 event emit, 리엑티비티도 적용되서 상위 컴포넌트에서 데이터를 수정해도 하위 폴더에도 적용이 된다 (반대도 마찬가지)


