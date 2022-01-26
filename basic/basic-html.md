# HTML(HyperText Markup Language)

<p align="center"><img src="https://github.com/limseongeun/frontend-knowhow/blob/main/basic/images/img_htm5_logol.png" alt=""></p>

프론트엔드개발을 시작할 때 가장 처음으로 익혀야 하는 언어로, 웹페이지에 들어갈 내용을 웹 브라우저가 인식할 수 있도록 **구조화 할 때 사용**합니다. 건축으로 보자면 가장 중요한 **건물의 뼈대 역할**이라고 할 수 있습니다. HTML을 실전에서 사용하기 위한 꼭 필요한 내용을, 언어의 이해를 위한 **정의**, 언어를 사용하기 위한 **코딩규칙**, 주로 많이 사용하는 **주요 태그**, 내용을 토대로 적용한 **HTML 샘플 페이지**로 정리를 하였습니다. 정리한 내용을 숙지하게 되면 바로 웹페이지 구조를 만들 수 있을 것입니다.

* <a href="#정의">정의</a>
* <a href="#코딩-규칙">코딩 규칙</a>
* <a href="#주요-태그">주요 태그</a>
* <a href="#HTML-샘플-페이지">HTML 샘플 페이지</a>

---

## 정의 <a id="정의"></a>

**HTML**은 웹 페이지 작성을 위한 표준 마크 업 언어로 **‘HyperText Markup Language’** 의 약자입니다. 현재는 월드 와이드 웹(**World Wide Web**, WWW, W3)에서 **‘HTML5’** 를 표준안으로 확정하여 웹사이트 제작 시 권고하고 있습니다. HTML은 웹 페이지의 구조를 설명하며, HTML 태그들(<a rel="noreferrer noopener" href="https://www.w3schools.com/tags/default.asp" target="_blank">w3schools</a> 기준 총124개)로 구성됩니다. 각각의 HTML 태그는 웹 페이지의 디자인(CSS)이나 기능(javascript)을 결정하는데 사용됩니다. 브라우저는 HTML 태그를 표시하지는 않지만 페이지의 컨텐츠를 렌더링합니다. 아래의 그림은 쉽게 HTML이 무엇인지 이해 할 수 있도록 실제 웹 사이트를 구성하는 HTML을 표시해 놓은 것입니다. 참고로 크롬 브라우저(Chrome)에서 **'F12' key'** 또는 **'옵션 &gt; 도구 더보기 &gt; 개발자도구'** 를 누르면 그림과 같이 **소스 보기**를 할 수 있습니다.

<img src="https://user-images.githubusercontent.com/13953651/150928925-da9596de-8e0d-477c-9565-f56bb068a72e.png" alt="" class="wp-image-1608" width="1024" height="907"/>
<p align="center"><sup>웹 사이트에서 컨텐츠 영역인 HTML 설명</sup></p>

<br>

## 코딩 규칙 <a id="코딩-규칙"></a>

### -  HTML  태그 형식

HTML 태그는 **꺾쇠 괄호로 묶인 요소** 이름입니다.

<p align="center"><code><strong>&lt;태그명 속성명="속성값"&gt; 콘텐츠가 여기에옵니다 ... &lt;/ 태그명 ></strong></code></p>


* HTML 태그는 일반적으로 **한 쌍으로** 같은 <code><strong>&lt;p></strong></code> 와 <code><strong>&lt;/p></strong></code> 로 사용해야 합니다.<br>예외로 <code><strong>&lt;img />, &lt;input />, &lt;br /></code></strong> 같은 몇몇 태그들은 하나의 태그로도 사용 가능합니다.
* 쌍의 첫 번째 태그는 **시작 태그**이고, 두 번째 태그는 **종료 태그**입니다.
* 종료 태그는 시작 태그처럼 작성되지만 태그 이름 앞에 **슬래시**가 삽입됩니다.
* 요소의 시작태그 안에 속성명과 속성값(id="html" class="common" href="#" 등)을 태그에 지정하여 사용할 수 있습니다.

<br >

### - HTML 문서

모든 HTML 문서는 <code><strong>&lt;!DOCTYPE html></strong></code> 문서 유형 선언으로 시작해야합니다.   
HTML 문서 자체로는 시작은 <code><strong>&lt;html></strong></code> 하고 <code><strong>&lt;/html></strong></code> 로 끝납니다.   
HTML 문서에서 보이는 부분은 <code><strong>&lt;body></strong></code> 와 <code><strong>&lt;/body></strong></code> 사이에 있습니다.

**예)**
```html
<!doctype html> // HTML5를 선언하기 위한 문서 정의
<html> // HTML 페이지의 루트 요소
  <head> // 문서에 대한 메타 정보를 포함
    <title>Hello HTML</title> // 문서의 제목을 명시
  </head>
  <body> // 눈에 보이는 페이지의 내용을 포함
    <h1>HTML?</h1> // 큰 제목을 정의
    <p>Hello World!</p> // 문단(단락)을 정의
  </body>
</html>
```
<p><a href="https://codesandbox.io/s/1-1-html-forked-0jpvd" target="_blank" rel="noopener noreferrer"><img class="alignnone" src="https://codesandbox.io/static/img/play-codesandbox.svg" alt="Edit 1-1. html" width="201" height="42" /></a></p>

<br>

### -  HTML  시각화 구조


아래는 HTML 페이지 구조의 시각화입니다.

<img src="https://user-images.githubusercontent.com/13953651/150938083-2da65eef-998e-4985-aa8f-a1e8868cab3e.png"/>

<br>

### - HTML 블록(Block) / 인라인(Inline) 태그

HTML 태그에는 **블록 레벨 요소** (Block-level Elements-사각형 덩어리) 와 **인라인 레벨 요소** (Inline-level Elements-직렬,일렬적인) 두 가지 범주로 나뉩니다.   
즉, 모든 HTML 요소는 블록 레벨 요소(줄바꿈 됨)이거나, 인라인 레벨 요소(줄바꿈 안 됨) 이거나 둘 중 하나라는 뜻입니다.   
각각의 대표적인 태그로는 <code><strong>&lt;div></strong></code> 태그는 **블록 요소**이고, <code><strong>&lt;span></strong></code> 태그는 **인라인 요소** 입니다.

| 블록 레벨 요소 (Block-level Element) | 인라인 레벨 요소 (Inline-level Element) |
|:---:|:---:|
| 줄바꿈 있고 앞뒤 태그에 다른 라인으로 출력 | 줄바꿈 없이 앞뒤 태그에 같은 라인으로 출력 |
| 내용과 상관없이 너비 항상 100% 태그 영역 (높이는 내용 크기에 맞춰 변화)  | 내용만큼 태그 영역 |
| 다른 블록, 인라인 태그를 담을 수 있음 <br> 예외) <code><strong>&lt;p></strong></code> 태그는 인라인 태그만 가능 | 인라인 태그만 담을 수 있음 <br> 예외) <code><strong>&lt;a></strong></code> 태그는 HTML5부터 내부 블록 태그 작성 가능 |
| 너비, 높이, 여백 설정 가능 | 너비, 높이, 여백(가로만 가능) 설정 불가능 |
| <code><strong>&lt;address></strong></code>, <code><strong>&lt;article></strong></code>, <code><strong>&lt;aside></strong></code>, <code><strong>&lt;audio></strong></code>, <code><strong>&lt;blockquote></strong></code>, <code><strong>&lt;canvas></strong></code>, <code><strong>&lt;dd></strong></code>, <code><strong>&lt;div></strong></code>, <code><strong>&lt;dl></strong></code>, <code><strong>&lt;fieldset></strong></code>, <code><strong>&lt;figcaption></strong></code>, <code><strong>&lt;figure></strong></code>, <code><strong>&lt;footer></strong></code>, <code><strong>&lt;form></strong></code>, <code><strong>&lt;h1></strong></code>, <code><strong>&lt;h2></strong></code>, <code><strong>&lt;h3></strong></code>, <code><strong>&lt;h4></strong></code>, <code><strong>&lt;h5></strong></code>, <code><strong>&lt;h6></strong></code>, <code><strong>&lt;header></strong></code>, <code><strong>&lt;hgroup></strong></code>, <code><strong>&lt;hr></strong></code>, <code><strong>&lt;noscript></strong></code>, <code><strong>&lt;ol></strong></code>, <code><strong>&lt;output></strong></code>, <code><strong>&lt;p></strong></code>, <code><strong>&lt;pre></strong></code>, <code><strong>&lt;section></strong></code>, <code><strong>&lt;table></strong></code>, <code><strong>&lt;ul></strong></code>, <code><strong>&lt;video></strong></code> 등 | <code><strong>&lt;a></strong></code>, <code><strong>&lt;abbr></strong></code>, <code><strong>&lt;acronym></strong></code>, <code><strong>&lt;b></strong></code>, <code><strong>&lt;bdo></strong></code>, <code><strong>&lt;big></strong></code>, <code><strong>&lt;br/></strong></code>, <code><strong>&lt;button></strong></code>, <code><strong>&lt;cite></strong></code>, <code><strong>&lt;code></strong></code>, <code><strong>&lt;dfn></strong></code>, <code><strong>&lt;em></strong></code>, <code><strong>&lt;i></strong></code>, <code><strong>&lt;img></strong></code>, <code><strong>&lt;input></strong></code>, <code><strong>&lt;kbd></strong></code>, <code><strong>&lt;label></strong></code>, <code><strong>&lt;map></strong></code>, <code><strong>&lt;object></strong></code>, <code><strong>&lt;q></strong></code>, <code><strong>&lt;samp></strong></code>, <code><strong>&lt;small></strong></code>, <code><strong>&lt;script></strong></code>, <code><strong>&lt;select></strong></code>, <code><strong>&lt;span></strong></code>, <code><strong>&lt;strong></strong></code>, <code><strong>&lt;sub></strong></code>, <code><strong>&lt;sup></strong></code>, <code><strong>&lt;textarea></strong></code>, <code><strong>&lt;tt></strong></code>, <code><strong>&lt;var></strong></code> 등 |

<br>

## 주요 태그 <a id="주요-태그"></a>

### - Layout

#### HTML &lt;! DOCTYPE> 선언

<code><strong>&lt;!DOCTYPE></strong></code> 선언은 **문서 유형**을 나타내며 웹 페이지에 브라우저를 올바르게 표시 하는 데 도움이됩니다.   
페이지 상단 (HTML 태그 이전)에 **한 번만** 나타내야 합니다.   
<code><strong>&lt;!DOCTYPE></strong></code> 선언은 대소 문자를 구분하지 않습니다.    
<code><strong>&lt;!DOCTYPE></strong></code> HTML5 의 선언은 다음과 같습니다.

**예)**
```html
<!doctype html>
```
<br>

#### HTML &lt;html> 루트

<code><strong>&lt;html></strong></code> 태그는 HTML 문서에서 **최상위 루트**를 나타냅니다.  
<code><strong>&lt;html></strong></code> 태그는 HTML 문서 내 다른 모든 HTML 요소의 컨테이너입니다. (단, <code><strong>&lt;!DOCTYPE></strong></code> 태그 제외)     
참고로 검색 엔진과 브라우저를 지원하기 위한 웹 페이지의 언어를 선언하려면 항상 태그 내부에 lang 속성을 포함해야 합니다.   

<br>

#### HTML &lt;head> 메타데이터 정보

<code><strong>&lt;head></strong></code> 태그는 메타데이터(데이터에 대한 데이터)의 영역이며 <code><strong>&lt;html></strong></code>  태그와 <code><strong>&lt;body></strong></code>  태그 사이에 배치됩니다.   
메타데이터는 **HTML 문서에 대한 정보**를 담고 있는 데이터이며, 웹 페이지 상에서는 표시되지 않습니다.   
메타데이터는 일반적으로 document title, character set, styles, scripts, and other meta 정보를 정의합니다.   
다음 요소는 <code><strong>&lt;head></strong></code>요소 내부에 들어갈 수 있습니다.

* <code><strong>&lt;title></strong></code> (모든 HTML 문서에 필요)
* <code><strong>&lt;style></strong></code>
* <code><strong>&lt;base></strong></code>
* <code><strong>&lt;link></strong></code>
* <code><strong>&lt;meta></strong></code>
* <code><strong>&lt;script></strong></code>
* <code><strong>&lt;noscript></strong></code>

<br>

#### HTML &lt;title> 문서 제목

<code><strong>&lt;title></strong></code> 태그는 문서의 **제목**을 정의하며, 내용은 텍스트 전용이어야 하며 브라우저의 상단 제목 표시줄이나 페이지의 탭에 표시됩니다.   
<code><strong>&lt;title></strong></code> 태그는 HTML 문서에 꼭 필요합니다!   
페이지 제목의 내용은 **검색엔진 최적화(SEO)** 에 매우 중요하며, 검색 엔진 알고리즘에서 검색 결과에 페이지를 나열할 때 순서를 결정하는 데 사용됩니다.

<code><strong>&lt;title></strong></code> 요소 :

* 브라우저 도구 모음에서 제목 정의
* 즐겨찾기에 추가될 때 페이지의 제목 제공
* 검색 엔진 결과에 페이지 제목 표시

좋은 문서 제목을 만들기 위한 팁은 아래와 같습니다.

* 제목을 가능한 한 정확하고 의미 있게 만드는 게 중요!
* 더 길고 설명적인 제목을 사용 (한 단어 또는 두 단어로 된 제목은 되도록 피함)
* 검색 엔진은 제목의 약 50-60자를 표시하므로 그보다 긴 제목을 사용하지 않도록 함
* 단어 목록만 제목으로 사용하지 않도록 함 (검색 결과에서 페이지의 위치가 줄어들 수 있음)

<br>

#### HTML &lt;body> 본문

<code><strong>&lt;body></strong></code> 태그는 문서의 **본문**을 정의하며, HTML 문서에 하나의 요소만 있을 수 있습니다.   
<code><strong>&lt;body></strong></code> 요소에는 제목, 단락, 이미지, 하이퍼링크, 표, 목록, 입력 양식 등과 같은 HTML 문서의 모든 내용이 포함됩니다.   

**예) &lt;html>, &lt;head>, &lt;title>, &lt;body>**
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Title of the document</title>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

<br>

#### HTML &lt;header> 소개

<code><strong>&lt;header></strong></code> 요소는 **소개 콘텐츠 또는 네비게이션 링크 집합의 컨테이너**를 나타냅니다.   
<code><strong>&lt;header></strong></code> 요소에 여러 요소가 있을 수 있지만, <code><strong>&lt;footer></strong></code>, <code><strong>&lt;address></strong></code> 또는 다른 요소 <code><strong>&lt;header></strong></code>는 <code><strong>&lt;header></strong></code>내에 배치할 수 없습니다.   
<code><strong>&lt;header></strong></code> 요소 :   

* 하나 이상의 제목 요소(<code><strong>&lt;h1></strong></code> - <code><strong>&lt;h6></strong></code>)
* 로고 또는 아이콘
* 저작권 정보
* 웹 페이지 상단 영역
  
<br>

#### HTML &lt;nav> 네비게이션

<code><strong>&lt;nav></strong></code> 태그는 **네비게이션 링크 집합**을 정의합니다.   
<code><strong>&lt;nav></strong></code> 태그는 메뉴, 목차 등 네비게이션 링크의 주요 블록에만 사용됩니다.
장애(시각)가 있는 사용자를 위한 스크린 리더와 같은 브라우저는 이 요소를 사용하여 콘텐츠의 초기 렌더링을 생략할지 여부를 결정할 수 있습니다.

<br>
  
#### HTML &lt;footer> 바닥글

<code><strong>&lt;footer></strong></code> 태그는 문서 또는 섹션의 **바닥글**을 정의합니다.   
<code><strong>&lt;footer></strong></code> 요소는 하나의 문서에 여러 개가 있을 수 있습니다.
<code><strong>&lt;footer></strong></code> 요소 :

* 저작권 정보
* 연락처 및 주소 정보
* 사이트맵
* 맨 위로 링크로 돌아가기
  
<br>

#### HTML &lt;main> 주요 내용

<code><strong>&lt;main></strong></code> 태그는 문서의 **주요 내용**을 지정합니다.   
<code><strong>&lt;main></strong></code> 요소의 내부 내용은 고유해야 하며, 문서에서 사이드바, 탐색 링크, 저작권 정보, 사이트 로고 및 검색 양식과 같은 반복되는 콘텐츠를 포함해서는 안 됩니다.   
<code><strong>&lt;main></strong></code> 태그는 문서에서 2개 이상 있어서는 안 되며, <code><strong>&lt;article></strong></code>, <code><strong>&lt;aside></strong></code>, <code><strong>&lt;footer></strong></code>, <code><strong>&lt;header></strong></code> 또는 <code><strong>&lt;nav></strong></code> 요소의 자손이 아니어야 합니다.

<br>

#### HTML &lt;article> 독립적인 기사

<code><strong>&lt;article></strong></code> 태그는 **자체적이고, 독립적인 콘텐츠**를 지정합니다.   
<code><strong>&lt;article></strong></code> 요소 :

* 포럼 게시물
* 블로그 포스트
* 뉴스 기사

<br>

#### HTML &lt;section> 섹션

<code><strong>&lt;section></strong></code> 태그는 문서 내에 **주제와 관련된 섹션**을 정의합니다.   
<code><strong>&lt;article></strong></code> 요소의 주로 자식 요소로 hn(h1~h6)태그 와 일반적인 콘텐츠가 포함됩니다.

<br>

#### HTML &lt;aside> 일부 콘텐츠

<code><strong>&lt;aside></strong></code> 태그는 배치된 콘텐츠 외에 **일부 콘텐츠**를 정의하며, 주변 콘텐츠와 간접적으로 관련되어야 합니다.  
<code><strong>&lt;aside></strong></code> 태그는 문서의 **사이드바**로 배치되는 경우가 많습니다.    

**예) &lt;header>, &lt;nav>, &lt;footer>, &lt;main>, &lt;article>, &lt;section>, &lt;aside>**
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Title of the document</title>
  </head>
  
  <body>
  
    <header>
      <h1>Browsers</h1>
      <nav>
          <a href="/Google Chrome/">Google Chrome</a> |
          <a href="/Mozilla Firefox/">Mozilla Firefox</a> |
          <a href="/Microsoft Edge/">Microsoft Edge</a> |
      </nav>
    </header>

    <main>
      <section>
        <h2>Google Chrome</h2>
        <p>Google Chrome is a web browser developed by Google, released in 2008. Chrome is the world's most popular web browser today!</p>
      </section>

      <section>
        <h2>Mozilla Firefox</h2>
        <p>Mozilla Firefox is an open-source web browser developed by Mozilla. Firefox has been the second most popular web browser since January, 2018.</p>
      </section>

      <section>
        <h2>Microsoft Edge</h2>
        <p>Microsoft Edge is a web browser developed by Microsoft, released in 2015. Microsoft Edge replaced Internet Explorer.</p>
      </section>

      <aside>
        <article>
          <h2>Epcot Center</h2>
          <p>Epcot is a theme park at Walt Disney World Resort featuring exciting attractions, international pavilions, award-winning fireworks and seasonal special events.</p>
        </article>
      </aside>
    </main>

    <footer>
      <p>Author: Hege Refsnes</p>
      <p><a href="mailto:hege@example.com">hege@example.com</a></p>
    </footer>

  </body>
</html>
```
<p><a href="https://codesandbox.io/s/basic-html-layout-9n2g0" target="_blank" rel="noopener noreferrer"><img class="alignnone" src="https://codesandbox.io/static/img/play-codesandbox.svg" alt="Edit basic-html-layout. html" width="201" height="42" /></a></p>

<br>

### - Contents

#### HTML <code><strong>&lt;hn></strong></code> 제목

<code><strong>&lt;h1></strong></code> ~ <code><strong>&lt;h6></strong></code> 태그는 HTML 제목을 정의할 때 쓰입니다.   
<code><strong>&lt;h1></strong></code> 은 가장 중요한 **제목**을 정의할 때 쓰이며, 문서에 **꼭 하나 이상**은 있어야 합니다.   
<code><strong>&lt;h6></strong></code>은 가장 나중 제목을 정의할 때 쓰입니다.

**예)**
```html
<h1>제목1</h1>
<h2>제목2</h2>
<h3>제목3</h3>
<h4>제목4</h4>
<h5>제목5</h5>
<h6>제목6</h6>
```
<br>

#### HTML <code><strong>&lt;p></strong></code> 단락

<code><strong>&lt;p></strong></code> 태그는 HTML 단락을 정의할 때 쓰입니다.

**예)**
```html
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>
```

<br>

#### HTML <code><strong>&lt;div></strong></code> 구분

<code><strong>&lt;div></strong></code> 태그는 HTML 문서에서 구분 또는 영역을 정의합니다.   
<code><strong>&lt;div></strong></code> 태그는 HTML 요소의 컨테이너로 사용하고, 그런 다음 CSS로 스타일을 지정하거나 JavaScript로 조작합니다.   
<code><strong>&lt;div></strong></code> 태그는 모든 종류의 콘텐츠를 내부에 포함 가능하며, id 또는 class 속성을 사용하여 쉽게 스타일을 지정할 수 있습니다.   

**예)**
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Title of the document</title>
    <style>
    .myDiv {
      border: 5px outset red;
      background-color: lightblue;
      text-align: center;
    }
    </style>
  </head>
  
  <body>
    
    <div class="myDiv">
      <h2>This is a heading in a div element</h2>
      <p>This is some text in a div element.</p>
    </div>

  </body>
</html>
```
<p><a href="https://codesandbox.io/s/basic-html-div-5pxlc" target="_blank" rel="noopener noreferrer"><img class="alignnone" src="https://codesandbox.io/static/img/play-codesandbox.svg" alt="Edit basic-html-div. html" width="201" height="42" /></a></p>

<br>

#### HTML <code><strong>&lt;span></strong></code> 단락

<code><strong>&lt;span></strong></code> 태그는 문서의 일부를 마크업하는 데 사용되는 인라인 컨테이너입니다.

**예)**
```html
<p>This is a <span style="color:blue">blue</span> paragraph.</p>
```

*****
### [목록으로 이동](README.md)
### [다음 - CSS(Cascading Style Sheet)](basic-css.md)

*****
### [홈으로 이동](https://github.com/limseongeun/frontend-knowhow)
