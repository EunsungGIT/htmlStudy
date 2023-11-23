git&github 순서
* 초기 디렉터리 생성 시 순서
1. git init 저장소 등록
2. git branch -M main
    master -> main으로 변경
3. git remtoe add origin HTTPS 주소 붙여넣기
    origin == gitHub HTTPS 주소 별칭
---------------------------------------------------------
* 초기 디렉터리 생성 후 작업 진행 시 순서
1. git add .
    .이란? == 현재 디렉터리 안 모든 파일과 폴더를 뜻함.
2. git commit -m 'message'
    현재 스테이징된 파일의 기록명을 작성(영어, 한글 모두 그낭, 짧게 키워드 위주로 작성하기)
    ex) 쇼핑몰 상품 페이지를 만들었다면?
        git commit -m 'shp man-product end'
        git commit -m '쇼핑몰 남자복 완성'
3. git push origin main
    origin == gitHub 주소
    main == Local 내 컴퓨터 위치
    해석 == gitHub에 Local 작업물을 Push 하겠다.
---------------------------------------------------------
위 add -> commit -> push 순서 중간 중간 작업 확인 리눅스 명령어
1. git status
    Local과 Staging 상태에서 작업물의 등록 상태 체크
2. git log
    commit과 Push 상태에서 작업물의 Commit 기록과 업로드 정보 체크
---------------------------------------------------------
* 블록태그(block Tag) & 인라인태크(inline Tag)
1. 블록 (큰 레이아웃 개념, 폭 100%, 새로운 행 배치)
2. 인라인 (작은 요소 개념, 폭 자기 자신만큼 인식, 옆으로 배치)
---------------------------------------------------------
# H1~H6 Tag(block)
* 제목 태그는 검색 키워드 역할을 하며 페이지 내에서 대/중/소 제목 역할을 한다.
* H1이 가장 중요한 제목이며 H1, H2, H3 위주로 많이 사용한다.
---------------------------------------------------------
# p Tag(block)
* 단락(내용)태그로 제목 아래 내용을 구성할 때 이용한다.
---------------------------------------------------------
# em, strong Tag(inline)
* 강조의미를 가진 em, strong은 블록 내에서 강조처리를 할 때 사용한다.
* 제목 태그(h)안에는 em, strong을 사용하지 않는다.
----------------------------------------------------------------------
# <11월 22일 tag 정리> 
# sub sup 아래첨자 , 위첨자(inline)
# del 교체, 삭제 텍스트 (inline)
# blockquote 긴 인용문 (block)
# q 짧은 인용문 (inline)
# code 화면에 코드 표시 (inline)
# address 연락처 및 주소 정보 (block)
* address 자식, 자손으로는 (inline) 요소만 배치할 수 있다.
# hr 수평선(block)
----------------------------------------------------------------------
11월 22일 
blockquote 긴 인용문 

나무위키에 고양이 소개 할거면
폭 넓이 100 밑으로 떨어지는 것 

단락 전체 중 일부 q 

전체가 인용문이면 block

출처 남기기에도 이용한다.
출저 주소.
------------------------------------------------------------------------

HTTP 웹프로토콜 관련 된 정보 

https://velog.io/@fnrkp089/HTTP%ED%86%B5%EC%8B%A0-%ED%86%B5%EC%8B%A0-%ED%94%84%EB%A1%9C%ED%86%A0%EC%BD%9C


-------------------------------------------------------------------------

code <p>웹 색상 코드 중 노랑색을 뜻하는 코드는<code>ffff00
      </code>이다.</p>

<code> 태그는 컴퓨터 코드(code)의 일부분을 나타낼 때 사용합니다.

 

이때 컴퓨터 코드의 일부분이란 XML 요소의 이름이나 파일 이름, 컴퓨터 프로그램의 코드, 또는 컴퓨터가 인식할 수 있는 어떤 문자열이라도 될 수 있습니다.


-------------------------------------------------------------------------

address 연락처, 회사소개, 고객센터 

웹사이트의 관련 연락처, 소개, 고객센터 정보등을 담을 때 사용합니다.
다른 블록을 자식 또는 자손으로 배치할 수 없습니다.
footer 영역에 주로 사용합니다. 

inline만 사용가능하다. 

ex) 쿠팡 밑에 

내 사이트에 관련된 정보만 넣어준다. 
협력업체에 대한 정보에는 사용안하고 일반적인 h or p - > 그냥 내용 일 뿐이다.

----------------------------------------------------------------------------
hr 
----------------------------------------------------------------------------

a tag (b,i 둘 다 )
html <a>요소는 href 속성을 통해서 다른 페이지나 같은 페이지의 오느 위치,파일, 이메일 주소와 그 외 다른 URL로 연결할 수 있는 하이퍼링크를 만듭니다.

a안에 h가 들어 갈 수 있고 
h안에 a가 들어갈 수 있다. 

목록 5개면 

독자적으로 A5개에 P로 묶기
블록에 블록 

이미지 밑에 글자링크를 넣는다면 
PX A만 넣기 


선택되는건 A 다른건 P 아님 다른걸로 생각하기 


하이퍼 링크 태그 a

1. 절대경로 
*절대경로는 변하지 않는 주소로 쉽게 말해 흔히 알고 있는 웹 주소를 떠올리면 됩니다.
http://naver.com 네이버가 망하지 않으면 안 사라짐.
절대경로는 http:// 웹 프로토콜로 시작한다.

<a href="">
------------------------------------------------------
# inline image tag
    src 이미지 경로 속성의 값으로는 상대경로 방식으로 작성하는 것을 권장합니다.
    대체 텍스트 alt 속성을 필수로 작성해야 합니다.
    이미지 사용 시 의미전달이 필요한 이미지와 아닌 이미지를 구분해서 사용해야 합니다.
    <img src="url" alt="내용">
# block figure / inline figcaption
    <figure><img src="URL" alt=""><figcaption?>caption</figcaption></figure>