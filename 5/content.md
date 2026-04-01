#### CSS3 (Cascading Style Sheet 3)

- HTML 문서의 색이나 모양, 배치 등 외관을 꾸미는 언어

- HTML의 각 요소를 대상으로 스타일 지정

- HTML과 다른 문법 사용

- 파일 확장자 *.css

#### 스타일 시트 문법
```
span { color : #ff0000; font-size: 32px; } /*빨간색, 32px;*/
```
- 선택자 : HTML 문서에서 스타일 적용 대상이 되는 요소를 선택

- 프로퍼티 : 스타일 속성 이름, 약 200여개의 프로퍼티 있음

- 값 : 프로퍼티의 값

- 주석문 : 스타일 시트에 붙이는 설명문으로 /*...*/ 형식

- 스타일 시트는 대소문자 구분 없음

#### 스타일 시트 적용 방법

- 방법 1 : 개별 태그의 style 속성에 프로퍼티와 값으로 직접 스타일 지정

- 방법 2 : <style> 태그에 스타일 시트 문법으로 스타일을 작성

- 방법 3 : 별도로 작성된 스타일 시트 파일을 불러오기


#### CSS3 스타일은 부모 태그로부터 상속

- 자식 태그는 부모 태그의 스타일을 상속 받음

#### CSS 선택자(selector)

- HTML 문서에서 스타일 적용 대상이 되는 요소를 선택하는 기능, CSS 뿐만 아니라 jQuery, Node.js 등 다양한 모듈에서 사용

- 선택자의 종류
```
태그 이름 선택자
클래스 선택자
id 선택자
범용 선택자
속성 선택자
```

- 선택자의 조합
```
선택자 목록 : A, B - 선택자 A와 선택자 B
인접 형제 선택자 : A + B - 선택자 A 바로 다음에 위치한 형제 선택자 B
일반 형제 선택자 : A ~ B - 선택자 A 이후에 나타나는 형제 선택자 B
자식 선택자 : A > B - 선택자 A의 직계 자식 선택자 B
자손 선택자 : A B - 선택자 A의 자식 또는 자식의 자식 선택자 B
```

- 의사 클래스
```
마우스
:active - 마우스를 누르고 있는 상태
:hover - 마우스가 올라간 상태

폼 요소
:focus - 포커스를 받은 상태

링크 
:link - 방문하지 않은 상태의 링크
:visited - 방문한 상태의 링크

구조
:first-child - 형제 요소 중 첫번째 요소
:last-child - 형제 요소 중 마지막 요소
:nth-child(n) - 형제 요소 중 n번째 요소

블록
::first-letter - 블록형 태그의 첫 글자(:first-letter)
::first-line - 블록형 태그의 첫 라인

요소 추가
::after - 선택한 요소의 마지막 자식 요소 추가
::before - 선택한 요소의 첫번째 자식 요소 추가

기타
::marker - <li>의 마커 요소
::placeholder - placeholder 속성으로 출력되는 문자열
::selection - 사용자가 선택하여 반전되는 부분
```

#### 주요 프로퍼티

- 주요 프로퍼티에는 색 관련 프로퍼티, 텍스트 프로퍼티, 폰트 프로퍼티, 배경 프로퍼티 가 있다.

#### 색 관련 프로퍼티

- color: <color>;
- background-color: <color>;

#### 텍스트 프로퍼티
```
text-align : left|right|center|justify; /* 정렬 */
text-decoration : none|underline|line-through; /* 텍스트 꾸미기 */
text-indent : <length>|<percentage>; /* 들여쓰기 */
```

#### CSS3 표준 단위

- 모든 프로퍼티 값은 단위를 사용해야 함
```
em : 배수
% : 퍼센트
px : 픽셀 수
cm : 센티미터
mm : 밀리미터
in : 인치
pt : 포인터
pc : 피카소
deg : 각도
```

#### 폰트 관련 프로퍼티
```
font-family: <font name>[, <font name>]; /*폰트 종류*/
font-size: <font size>; /*폰트 크기*/
font-weight: normal|bold; /*폰트 굵기*/
font-style: normal|italic; /* 폰트 스타일 */
```