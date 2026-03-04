#### 클라이언트-서버 구조

- 클라이언트가 브라우저를 통해 서버에 요청(request)를 전달하고, 서버가 브라우저에게 응답(response)를 보내주고, 브라우저가 클라이언트에게 내용을 구성해서 보여준다(render).

#### URL(Uniform Resource Locator)

- 웹에서 인터넷 상의 고유한 자원의 위치를 표시하는 방법
```
<구성형식>
서비스프로토콜://서버주소:포트번호/경로/이름

ex. https://cafe.naver.com:80/swimming/...
    ftp://ftop.hufs.ac.kr/~...
```

- 내 로컬에서 파일의 경우는 절대주소가 아닌 상대주소이다.

#### DNS (Domain Name Service)

- DNS 서버에 도메인 이름을 질의하면 IP주소를 응답한다.
```
ex. www.devwooju.dev

<powershell>
    nslookup www.devwooju.dev

=>  서버:    UnKnown
    Address:  203.232.224.2

    권한 없는 응답:
    이름:    www.devwooju.dev
    Address:  15.165.117.125
```

#### 정적 웹페이지(Static Web) vs. 동적 웹페이지(Dynamic Web)

- 정적 웹페이지 : 언제나 동일한 고정된 데이터를 제공하는 웹페이지

- 동적 웹페이지 : 접속하는 상황에 따라 브라우저에 전송되는 데이터가 달라지는 웹 페이지, 일반적으로 DB를 참조하며 WAS(Web Applicaiton Server)를 통해 동적으로 페이지 작성

```
소프트웨어에서의 동적과 정적의 차이는 프로그램이 실행되면서 입력된 값에 맞춰서 출력값이 정해진다는 의미인데, 웹페이지에서의 동적과 정적의 의미도 마찬가지이다. 서버가 클라이언트로부터 요청을 받아서 동적으로 처리해 결괏값을 돌려준다는 의미이다.
```

#### 프론트엔드 vs. 백엔드

- 프론트엔드 프로그램 : 클라이언트에서 실행되는 프로그램

- 백엔드 프로그램 : 서버에서 실행되는 프로그램

```
간단히 말하면, 위와 같지만 조금 더 구체적으로 말하자면 프론트엔드는 일반적으로 사용자가 보는 화면을 구성하는 프로그램이고, 백엔드는 프로그램 화면 뒤에서 일어나는 로직을 처리해주는 프로그램이다.
```

#### 서버 프로그램 (백엔드 프로그램)

- WAS(Web Application Server)에서 웹페이지를 만드는 프로그램
=> Java, C3, Python, Ruby, JavaScript 등 다양한 언어로 개발
=> 그러나 웹개발을 쉽게 개발할 수 있도록 웹 프레임워크 사용

#### 웹 프레임워크

- 프레임워크 : 특정 분야/목적의 소프트웨어 개발의 뼈대 역할을 하는 것
ex. 웹 프레임워크 : Java Spring, Python Django, Python Falsk
    프론트엔드 프레임워크 : Angular JS, Vue.js, React

#### HTML (Hyper Text Markup Language)

- 마크업 언어 (Markup Language)
=> 인쇄 교정지의 '마크 업'에서 유래
=> 문장의 속성을 설정하는 마크업을 *태그*의 형태로 표시
=> 대표적인 마크업 언어 : SGML, HTML, XML

- 웹페이지를 작성하는 HTML
=> HTML 언어는 SGML 표준에 따라 정의
=> 텍스트 파일 형식으로 저장
=> 확장자 *.html 또는 *.htm으로 저장

#### 웹 표준 기술 HTML = HTML5 + CSS3 + JavaScript

- HTML5 : 웹페이지의 내용을 표현하는 마크업 언어

- CSS3(Cascading Style sheet level 3) : 웹페이지의 스타일을 정의하는 언어

- JavaScript : 웹페이지의 동작을 처리하는 스크립트 언어
=> 표준 명칭은 ECMASCript
=> 브라우저 뿐만 아니라 서버에서도 사용

- HTML5 주요 기능 
=> 멀티미디어 기능
=> 그래픽 기능
=> 통신 기능
=> 장치 접근
=> 오프라인 및 저장소
=> 웹의 성능 극대화 및 통합, Semantic Web(검색 엔진이 알아보기 쉽게 내용을 이해할 수 있게 만들어 둔 것)