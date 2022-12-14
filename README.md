# 과제 주요 사항 안내

## 1. 폴더 구조에 관해

   - 폴더 구조는 자유롭게 작성해주시면 됩니다.
   - 단, 해당 폴더가 왜 이런 구성을 갖추게 됐는지는 설명할 수 있어야 합니다.  
   - 별도의 README.md 파일을 만들어서 작성해주세요 ★  
     ㄴ 깃헙 레포지토리 팔 때 Add README.md 하지 말고 커밋 시에 같이 넣는 걸 추천.(충돌 방지)  

### - 과제 예시
  shared = 각 페이지 별로 경로를 주고 받는 라우터를 관리하기 위함.  
  redux  
  ┌ config = redux의 store의 설정을 관리하는 파일을 모아둠.  
  └ modules = redux에서 reducer의 설정을 관리하는 파일을 모아둠.  
  pages = 실제 유저들이 보게 될 화면 구성 파일들을 모아둠.  
  components/ui = 실제 유저들이 화면을 볼 때 공통적으로 적용될 UI 파일들을 모아둠.  
  features/todos/components = todoList와 관련한 기능들을 담당하는 컴포넌트들을 모아둠.  
  https://ko.reactjs.org/docs/faq-structure.html  

## 2. Ducks 구조에 관해
   https://velopert.gitbooks.io/react-redux/content/4-1-ducks.html  
   https://velog.io/@lllen/redux-s45cvers  
   참고합시다.  

## 3. 과제 화면
###   3-1. 메인 화면
   기존 과제 내용과 동일합니다. 단, 각 리스트에 '상세 보기' 페이지가 추가되었습니다.  

###   3-2. 상세 보기
   상세 페이지에서는 다음과 같은 내용들이 출력되어야 합니다.  

   - Todo의 ID
   - Todo의 제목
   - Todo의 내용
   - 이전으로 버튼 => 메인 화면으로 이동.  
     ★ .map 메소드는 반드시 key를 포함해야합니다.  
     ★ todos.length 사용해서 id를 생성하는 걸 지양해야함. = 왜 그렇게 되는지 알아야함.  
     ★ 대체제로 쓰는게 react-id-generator인 듯 하다.  

## 4. 설치해야 할 패키지

   - npx create-react-app (경로) --template redux (기본적으로 react-redux도 설치됩니다)  
   - npm install react-router-dom
   - npm install styled-components
   - npm install react-id-generator

## 5. 읽는 순서?

   - 파일은 되도록 자유롭게 읽어도 되는데, 그래도 작성을 정리한 흐름은 아래와 같습니다.
   - index.js -> App.js -> Router.jsx -> components/ui 폴더의 Header.jsx, Layout.jsx -> pages 폴더의 Home.jsx (여기들은 단순한 내용이에요.)
   - 그 다음, redux의 config/configStore.js -> modules 폴더의 todos.js (redux의 내용을 알고 싶다면 여기서부터 시작입니다.)
   - 마지막으로 feature/todos/components의 Form.jsx, List.jsx -> 그리고 pages의 Details를 읽어주세요.

## 6. 참고 자료?

   - https://develop-neoguri.notion.site/Redux-0d0b0258fee04aaf8b7cd051cf10812f
   - https://develop-neoguri.notion.site/React-Redux-2b1fc175fe064338a16cdcf58dbfd1f8

## 7. 정리 후에 알아야할 사항.
   - 과제 내용에는 여러분들이 이 과제를 진행할 때 왜 폴더를 이렇게 구성했는지를 README.md 파일에 추가하라고 적혀있었습니다.
   - 과제 예시의 링크 등을 통해 보시고 자신만의 폴더 구조를 갖춘 뒤 이걸 왜 이렇게 구성했는지 고민하면서 정리해봅시다.
