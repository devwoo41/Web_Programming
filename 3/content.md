#### 표 작성을 위한 태그

- <table></table> 태그 - 표 전체를 담는 컨테이너

- <caption></caption> 태그 - 표 제목

- <tr></tr> 태그 - table, row 행

- <th></th> 태그 - table header, 제목 셀

- <td></td> 태그 - table data, 데이터 셀

#### HTML(HyperText Markup Language)

- 하이퍼텍스트 : 서로 연관된 문서나 텍스트 조각들을 연결

- 하이퍼미디어 : 텍스트 뿐 아니라 이미지, 오디오, 비디오 등의 멀티미디어 정보가 서로 연결

#### 노드, 링크, 앵커

- 노드 : URL로 구분하는 정보 단위, HTML 문서 또는 멀티미디어 파일

- 링크 : 노드를 연결하는 구성요소, 링크를 통해 네비게이션을 구현

- 앵커 : 링크의 출발점이나 도착점을 의미

#### <a></a> 태그로 하이퍼링크 작성

- 링크의 출발점에서 도착점을 지정하는 요소
```
1. "URL" - 다른 페이지로 이동

2. "URL#앵커이름" - 다른 페이지 + 특정 위치 이동

3. "#앵커이름" - 현재 페이지 + 특정 위치 이동
```

- href: 도착점의 위치를 URL과 앵커이름으로 지정

- target : 도착점의 HTML 문서가 출력될 윈도우 이름 지정
```
_blank : 새로운 브라우저 윈도우(탭) 생성
_self : 현재 윈도우
_parent : 부모 윈도우
_top : 최상위 브라우저 윈도우
```

#### 웹 폼

- 웹 페이지에서 사용자 입력을 받는 폼
ex. 로그인, 등록, 검색, 예약, 쇼핑 등

#### 폼 요소

- 폼을 만드는 다양한 태그
ex. <input>, <textarea>, <select> 등

#### form 태그
```
<form name="폼이름" action="응용프로그램URL" method="GET|POST" enctype="인코딩타입" target="윈도우이름">

name : 폼 이름
action : 서버에서 실행되는 응용프로그램 URL
method : 폼 데이터를 서버에 전송하는 방식
    GET: action URL에 폼 데이터를 붙여서 전송
    POST: 요청 메시지의 바디에 폼 데이터 전송
enctype: 폼 데이터 인코딩 타입
    application/x-www-form-urlencoded : 기본값
    multipart/form-data " <input type="file">이 존재하는 경우 사용
    text/plain : 디버깅 용
target : 서버에서 전송 받은 문서를 출력할 윈도우
```

#### 데이터를 입력하는 폼 요소 <input>
```
<input type="폼 종류" name="요소 이름" value="초기텍스트" . . . >
```
- type : 폼의 종류 (디폴트 "text")

- name : 요소 이름, 서버로 전송되는 폼 데이터의 이름

- value : 초기값으로 입력되는 텍스트

- size : 입력 창의 크기 (디폴트 20)

- minlength, maxlength : 입력할 수 있는 최소, 최대 문자 개수

- pattern : 입력되는 텍스트의 문법을 정규 표현식으로 지정하여 유효성 검사 수행

- placeholder : 입력되는 내용의 힌트를 표시하는 문자열
