# 23.04.06 position 과제기록

##문제해결
header라는 영역안에 작업할 메뉴바를 nav로 묶어주고 각각의 영역을 확보했다.
nav에 최대 가로사이즈 1200px의 값을 설정해주니 header는 자식의 영향으로 가로사이즈를 갖게 되었다.
header에 position: fixed; 라는 값을 주어 본래의 성격을 바꿔주고 높이값과 배경색을 nav와 동일하게 주었다.
스크롤을 내려도 메뉴의 넓이와 상관없이 상단전체가 같은 색상으로 고정되어 있는것처럼 보였다.

##문제과정
1. 한번 해본 예제라서 쉽게 작업할 수 있을거란 착각을 했다
2. main에 공갈 div영역을 주어 포지션값을 주려고 했다가 실패 -> 가장 가까운 부모이상의 요소이니 header 영역으로 공갈 div 이동
3. header 안에서 구역을 나눠주기위해 기존 메뉴바에 들어가 내용을 nav로 묶어주었다. 공갈 div 포지션값을 주었으나 어떻게 해도 메뉴바 위에 고정되어 로고, 로그인등 모두 가려버렸다.
4. 그러다 문득 position: fixed; 이 값을주면 원래가지고있던 성격과 바뀌어 높이값을 줄 수 있다고 한것이 생각났다
5. 공갈 div를 삭제후, 상단의 문제해결 방법과 같이 진행했다

##현재 기쁨보다는 피곤이 더 크다. 졸린데 한번 손을대니 멈출 수가 없었다. 
