<h1>🤓 1주차 강의요약</h1>


<h3>[만들기]</h3>
<p>

    무엇인가를 만들기 전에, 미리 상상하고 계획해보는 과정이 필요하다.
    그 다음 상상한 웹 사이트를 만들때는 순서가 중요하다.

    이때 사람이 하는 일을 원인, 기계가 하는 일은 결과로 볼 수 있다.
    'code, source, 컴퓨터 언어'가 원인에 해당하고, '앱, 응용프로그램'등이 결과에 해당한다.
    코딩은 원인인 코드를 통해 결과를 만드는 것이라고 정리할 수 있다.

    HTML은 웹페이지를 만드는 코드이다. 웹에서의 결과는 웹페이지라고 한다.
    웹페이지의 그룹은 웹사이트이고, 기능이 많은 경우에는 웹앱이라고도 한다.
</p>

<h3>[웹? 인터넷?]</h3>
<p>

웹에 대해 더 알아보기에 앞서 인터넷과 웹을 구별해보자.

인터넷은 1960년대에 강력한 통신 시스템의 필요에 의해 개발되었다.<br>
웹은 1990년대에 스위스 입자물리연구소의 팀 버너스 리에 의해 탄생했다.<br>
    (주소창에 info.cern.ch를 넣어보자.. 이곳이 원시 웹이다..!) 

웹의 client와 server라는 개념을 알아보기 위해 예시 상황을 들어보자.<br>

    2개의 프로그램을 개발해 웹서버/웹브라우저라는 이름을 붙인다. 

    - 웹서버가 설치된 컴퓨터에는 info.cern.ch라는 주소를 부여하고 컴퓨터에 index.html이라는 파일을 저장한다. 
    - 웹브라우저가 설치된 컴퓨터에 http://info.cern.ch/index.html이라는 주소를 입력한다.
        그리고 엔터를 누르면..!!

     1. 웹브라우저가 설치된 컴퓨터는 인터넷을 통해 info.cern.ch라는 주소의 컴퓨터에게 전기적인 신호를 보낸다. 
        (index.html파일의 코드를 알고싶어요!!)
     2. info.cern.ch에 설치된 웹서버라는 프로그램이, 컴퓨터의 한 디렉토리에서 index.html이라는 파일을 찾는다. 
       -> 내용을 읽어 전기적인 신호로 바꾼다
       -> 웹브라우저가 설치된 컴퓨터에 신호를 보낸다.
     3. 웹브라우저가 설치된 컴퓨터에 index.html 코드가 도착하고, 웹브라우저는 코드를 읽어 화면에 출력한다.
        -> 웹브라우저가 설치된 컴퓨터는 정보를 요청한다. --> 웹브라우저: client
        -> 웹서버가 설치된 컴퓨터는 정보 요청에 응답한다.--> 웹서버:     server

인터넷과 웹의 관계를 쉽게 알아보자면, 도시와 건물로 비유할 수 있다. 
즉, 웹은 인터넷을 통해 정보를 표현하는 서비스의 일종이다!
</p>

<h3>[HTML - 태그]</h3>
<p>

HTML이라는 컴퓨터 언어의 사용법을 배운다는 것은 웹브라우저를 제어하는 방법을 배우는 것이다.<br>
HTML은 HyperText Markup Language이다.<br>
이때 HyperText는 Tag를 의미한다.<br>
아래는 HTML의 기본구성이다.

    !DOCTYPE html: 이 웹페이지가 HTML로 만들어졌다는 것을 표현하는 코드. 문서의 시작에 추가한다.
    
    html: body 태그와 head 태그를 감싸는 태그. 문서의 시작과 끝이다.
    head: 본문 부분의 태그
    meta: 문서와 관련된 여러가지 항목들을 지정하는 태그. 
            meta태그의 문자셋 설정을 이용해 인코딩 방식을 UTF-8로 설정하면, 
            한글뿐만 아니라 세상의 모든 언어를 표시할 수 있다.
    title: 문서(웹페이지)의 제목을 나타내는 태그. 
            검색엔진이 웹페이지를 분석할 때 가장 중요하게 생각하는 태그이다.
    body: 본문 태그
</p>
<p>
이렇듯 태그란 HTML 언어의 문법이다.<br>
태그는 일상에서 자주 사용하는 말과 비슷하다.

    h1~h6: 제목 태그이다. h1에서 h6으로 갈수록 글자의 크기가 작아진다. heading
    a: 하나의 페이지에서 다른 페이지를 연결할 때 사용하는 태그로, 하이퍼링크를 정의할때 사용하는 태그이다. Anchor.
    href: Hypertext Markup Language의 Hypertext Reference를 줄인 태그이다.
        -> target="_blank": _가 있으면 새 창에서 페이지 오픈, _가 없으면 현재 페이지에서 링크된 페이지로 전환
        -> title= 링크에 커서를 올리면 보여주는 페이지 정보
    img: 이미지를 삽입할때 사용하는 태그이다.
    p: 문단을 표현할때 사용하는 태그이다.
    strong: 글자를 진하게 표시해주는 태그이다.
    u: 글자에 밑줄을 그려주는 태그이다. (underline)
    li: list
    ul: 경계가 있는 list. unordered list
    ol: ordered list
        -> 태그의 중첩을 parent, child의 관계로 볼 수 있고, ul,ol은 parent 태그, li는 child 태그이다.
    br: 새로운 줄을 표현하는 태그이다. 
        무엇인가를 설명하는 태그가 아니어서 태그를 닫지 않는다. 
        단락을 변경할 때에는 <br>태그 보다는 <p>태그를 사용한다.
    style: 문서의 스타일 정보를 정의할 때 사용한다.

<h2>태그가 중요한 이유</h2>
1. HTML 태그를 잘 활용해야 검색 엔진 노출 가능성⬆️<br>
2. 웹의 핵심 철학 "접근성 & 개방성" HTML을 잘 활용하면 신체적 장애가 있는 사람에게도 동일한 정보 접근성 제공 가능<br><br>

++<br>
속성: 태그의 심화 문법<br>
-> img 태그를 사용할 때에는 어떤 이미지를 불러올 것인지에 대한 정보를 담은 src를 넣어야 정상적으로 작동한다.
<p>