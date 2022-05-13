# 뷰 컴포넌트

- ###### Vue.js 특징 중에 컴포넌트가 있음

- ## 컴포넌트란?
  
  화면의 영역을 영역별로 구분해서 코드로 관리할 수 있는 뷰의 기능
  
  (헤더, 컨텐츠 , 그리드 등등) 영역별로 구분, 컴포넌트간에 관게가 생긴다

- ## 컴포넌트 핵심
  
  - 재사용성
    
    코드 반복을 최대한 줄이고 코드를 기존에 써놨던 코드를 가지고 최대한 많은 화면들을 뽑아 낼 수 있다.

## Root 컴포넌트

- 인스턴스를 생성하면 그 인스턴스는 기본적으로 Root 컴포넌트가 됨
  
              Vue.component('app-header', {
  
                  template: '<h1>Header</h1>'
  
              });
  
  를 할당시 Root 컴포넌트 아래에 AppHeader라는 컴포넌트가 등록된다
  
  마찬가지로
  
              Vue.component('app-content', {
  
                  template: '<div>content</div>'
  
              });
  
  를 코드에 추가시 Root 컴포넌트 아래에 AppContent라는 컴포넌트가 등록된다


