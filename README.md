# study_JH
UI/UX 웹퍼블리셔 공부 중!!


## 230511 과제기록

__VANS 리디자인 웹구성__

    [ 리디자인 선정이유 ] 
    https://www.vans.co.kr/aboutVans
    현재 글과 유튜브 영상으로 이루어진 About Vans 페이지는 가독성이 떨어진다.
    반스 온라인 쇼핑몰에 비해 중요도가 떨어지는 페이지라서 단순하게 구성한 것이라 추축되지만, 
    동종업계 아디다스, 나이키 등에 비해 브랜드 소개페이지의 완성도가 낮아 보인다.
    브랜드 소개 페이지는 그 브랜드의 가치와 나아갈 방향을 소비자에게 전달하는 역할을 한다. 
    브랜드를 잘 느낄 수 있도록 리디자인하여 웹의 완성도를 높이고자 했다.

    [ 브랜드의 핵심 가치 3가지 ]
    1. 스케이트문화에서 이어져 온 반스 스토리 
    2. 다양한  콜라보레이션 
    3. 개인의 개성과 자유를 존중하는 반스 커스텀



## 230504 과제기록

__PanStar 홈페이지 연습__

    https://www.panstar.co.kr/
    현재까지 공부한 내용으로만 홈페이지 레이아웃을 잡았다.
    전체적인 구조를 정리하고 한 부분씩작업을 해나가는 재미가 있었다.


## 230502 과제기록

__오늘의 고민1: 웹으로 확인한 화면과 모바일로 확인한 화면이 다르다?!__

    css 작성시 단위값을 잘 설정해야 한다는 걸 깨달았다.
    -> 보여지는 화면값에 따라 vw, vh, %, px 등 선택을 잘했어야 함을 깨달았다.

__오늘의 고민2: 깃허브 페이지 404에러 발생__

    당황하지않고 구글에 검색해보았는데 원인이 3가지정도로 나왔다. 
    1. 호스팅한지 시간이 별로 안지났을때: 호스팅 한지 몇 분 밖에 안지났을 경우 조금 더 기다려 본다.
    2. 메인 html 이름이 잘못됐을 경우: 처음 시작시 들어가는 html이름이 index.html이 아니면 404 에러가 뜰수있다. 
       방법1) 처음 시작 html이름을 index.html로 바꾼다.
       방법2) 배포하는 링크 이름 뒤에 시작 시 html이름을 쓴다. https://[깃허브 아이디].github.io/[저장소 이름]/[시작시 html 이름]
    3. 이미지, 혹은 어떤 파일의 경로가 잘못됐을 경우: 확인하여 경로를 수정해준다.
    -> 나의 경우 1번의 이유였다. 시간이 지나자 해결되었다
   

## 230426 과제기록

__오늘의 고민1:  클릭시 움직임을 줄때 선택자를 어떻게 작성할 것인가__

    움직임을 주고자 하는 영역이 input과 형제관계로 동등하게 있는 경우, 인접형제 선택자를 사용하여 transform 적용
    -> 선택자를 잘 찾으면 작업시간이 줄어든다는 것을 다시 한번 깨달았다.


## 230412 과제기록

__오늘의 고민 1:  background 축약에서 이미지 크기 수정__

    축약형을 활용하여 이미지를 원하는 비율의 사이즈로 한번에 적용하고 싶다.
    -> background: 컬러 url() no-repeat x축 y축 / 사이즈; 
    -> 사이즈 위치에 contain을 적용하니 원본 이미지 그대로가 적용되었다.
    -> 사이즈 조절을 %로 주니 원본 비율을 유지하면서 알맞게 사이즈가 적용된걸 확인했다.

__오늘의 고민 2:  input 중앙정렬__

    form안에서 input 중앙 정렬
    -> input 타입은 인라인 요소라서 한줄에 나란히 생성되는 것을 확인
    -> <p></p>태그 사이에 input을 작성해서 블록성격을 주었다.
    -> text-align 으로 가로 중앙 정렬은 되었으나 세로 중앙정렬은 되지 않았다.
    -> 다른 방법을 시도했으나 실패 (실패 사례: display: block;을 주어 margin: 숫자px auto; 등을 주었지만 실패)
    -> p태그의 사이즈를 개발자도구에서 확인 후, 폼의 높이값과 내가 원하는 위치 확인후 padding-top에 값을 입력
    -> 보기엔 원하는 이미지와 비슷하나 이 방법이 맞는지 의구심이 들어 구글에 찾아봄. 원하는 답은 못찾았다.
    -> 계속 고민해보면 언젠간 깨달음이 있지 않을까 기대해본다 


## 230411 과제기록

__오늘의 고민:  a태그 5개가 함께하는 메뉴바의 양쪽 여백이 있게 중앙 정렬__

    예시때마다 중앙 정렬에 대한 어려움을 느끼는데, 익숙해 질 쯤 새로운 고민을 맞이한다.
    -> <menu></menu>를 사용하여 순서없는 목록태그로 <a>태그를 만들어 주고 float: left; 로 정렬을 했다.
    -> 예제 이미지를 포토샵에서 확인하여 높이값을 지정해주고 가로값도 주었다.
    -> 그 상태에서 margin값이나 text-align으로 중앙 정렬이 되지 않았다. 한참을 이곳저곳에 적용해 보았다.
    -> 결국 이미지처럼 보이기만 하면 된다는 생각을 했다.
    -> <menu>태그의 내용을 <nav>로 감싸주어 높이값, 가로값은 100% 주고 menu li와 동일한 색상값을 주었다.
    -> <menu>의 가로값을 <nav>보다 작게 설정하여 margin: 0 auto; 로 중앙정렬 성공. 
    -> 동일한 배경색으로 하나의 메뉴바의 양쪽 끝 여백을 넓게 두고 중앙정렬된것 처럼 보이게 되었다

<details>
    <summary>nav태그</summary>
    <p>메뉴, 목차, 인덱스 등 다른 페이지 또는 현재 페이지의 다른 부분과 연결되는 네비게이션 링크들의 집합을 정의할 때 사용</p>
</details>



## 230410 과제기록(230411 추가작성)

__오늘의 고민:  git push 오류__

    과제 진행 후, 로컬 레파지토리에서 깃허브로 푸쉬를 진행했으나 되지 않았다.
    -> 구글에서 오류 내용을 복사하여 검색
    -> README.md 파일에 대한 오류라고 한다. 
    -> 강제로 파일을 등록할 수 있는 git push -u origin +main 으로 푸쉬를 강제 진행하니 깃허브에서 확인이 되었다.
    -> README.md 파일에 오류내용과 해결과정을 기록
    -> 230411 확인하니 README.md 파일에서 10일에 작성한 내용을 확인할 수 없었다
    -> 11일에 진행하기전, git pull을 하여 깃허브와 로컬 레피지토리를 동기화해주었다.
    -> 11일 당일 푸쉬 진행시 오류메세지가 뜨지 않았다.

