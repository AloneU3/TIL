# Vue 인스턴스

- #### new Vue();
  
  Vue로 개발할 때 필수로 생성해야하는 코드

- #### var vm = new Vue();
  
  #### console.log(vm);
  
  인스턴스 생성 후 인스턴스 안에 어떤 속성과 API가 있는지 콘솔창에서 확인가능
  
  (크롬 개발자 도구 console에서 확인 가능)

## Vue 인스턴스 생성 후

- el: '#(div id 입력)'으로 꼭 연결헤 줘야한다. 입력 안할시 아무리 많은 코드를 입력한다 해도 적용이 안됨.



# 인스턴스와 생성자 함수

- 생성자 함수
  
  function Pet(name, age) {
  
      this.name = name;
  
      this.age = age;
  
  }
  
  위와 같이 함수를 만들면 이제 인스턴스를 찍어낼 수 있다
  
  name과 age에 입력한 값을 Pet(name, age)로 넘겨줌

        

        var p = new Pet('poyo', '2'); 

        p라는 객체에 정보를 담음

        위와 같이 함수를 이용해서 어떤 정보를 담은 객체를 생성하는게 생성자 함수에 

        객체생성 패턴이다.



- Vue를 생성자 함수 형태로 찍어내는 이유 (var vm = new Vue를 사용하는 이유)
  
  예로
  
  function Vue() {
  
      this.hi1 = function() {
  
               console.log('hello');
  
      }
  
  }
  
  hi1이라는 함수를 미리 정의할 수 있다
  
  내가  ver vm = new Vue(); 를 생성할때마다
  
  그 객체 안에는 내가 미리 정의한 hi1이라는 함수가 들어가 있는것
  
  vm.hi1();를 입력하면 내가 정의한 hello가 출력된다



       즉 생성자 함수로 내가 Vue에서 API나 속성들을 다 정의해 놓고 나는 만들거 놓은 것을

       가져다 쓰거나 재사용하는 패턴을 취할 수 있다.

        
