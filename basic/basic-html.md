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
| <code><strong>&lt;address></strong></code>, <code><strong>&lt;article></strong></code>, <code><strong>&lt;aside></strong></code>, <code><strong>&lt;audio></strong></code>, <code><strong>&lt;blockquote></strong></code>, <code><strong>&lt;canvas></strong></code>, <code><strong>&lt;dd></strong></code>, <code><strong>&lt;div></strong></code>, <code><strong>&lt;dl></strong></code>, <code><strong>&lt;fieldset></strong></code>, <code><strong>&lt;figcaption></strong></code>, <code><strong>&lt;figure></strong></code>, <code><strong>&lt;footer></strong></code>, <code><strong>&lt;form></strong></code>, <code><strong>&lt;h1></strong></code>, <code><strong>&lt;h2></strong></code>, <code><strong>&lt;h3></strong></code>, <code><strong>&lt;h4></strong></code>, <code><strong>&lt;h5></strong></code>, <code><strong>&lt;h6></strong></code>, <code><strong>&lt;header></strong></code>, <code><strong>&lt;hgroup></strong></code>, <code><strong>&lt;hr></strong></code>, <code><strong>&lt;noscript></strong></code>, <code><strong>&lt;ol></strong></code>, <code><strong>&lt;output></strong></code>, <code><strong>&lt;p></strong></code>, <code><strong>&lt;pre></strong></code>, <code><strong>&lt;section></strong></code>, <code><strong>&lt;table></strong></code>, <code><strong>&lt;ul></strong></code>, <code><strong>&lt;video> 등 | <code><strong>&lt;a></strong></code>, <code><strong>&lt;abbr></strong></code>, <code><strong>&lt;acronym></strong></code>, <code><strong>&lt;b></strong></code>, <code><strong>&lt;bdo></strong></code>, <code><strong>&lt;big></strong></code>, <code><strong>&lt;br/></strong></code>, <code><strong>&lt;button></strong></code>, <code><strong>&lt;cite></strong></code>, <code><strong>&lt;code></strong></code>, <code><strong>&lt;dfn></strong></code>, <code><strong>&lt;em></strong></code>, <code><strong>&lt;i></strong></code>, <code><strong>&lt;img></strong></code>, <code><strong>&lt;input></strong></code>, <code><strong>&lt;kbd></strong></code>, <code><strong>&lt;label></strong></code>, <code><strong>&lt;map></strong></code>, <code><strong>&lt;object></strong></code>, <code><strong>&lt;q></strong></code>, <code><strong>&lt;samp></strong></code>, <code><strong>&lt;small></strong></code>, <code><strong>&lt;script></strong></code>, <code><strong>&lt;select></strong></code>, <code><strong>&lt;span></strong></code>, <code><strong>&lt;strong></strong></code>, <code><strong>&lt;sub></strong></code>, <code><strong>&lt;sup></strong></code>, <code><strong>&lt;textarea></strong></code>, <code><strong>&lt;tt></strong></code>, <code><strong>&lt;var></strong></code> 등 |

<br>

## 주요 태그 <a id="주요-태그"></a>

### - Layout

####  - HTML &lt;! DOCTYPE> 선언

<code><strong>&lt;!DOCTYPE></strong></code> 선언은 문서 유형을 나타내며 웹 페이지에 브라우저를 올바르게 표시 하는 데 도움이됩니다.   
페이지 상단 (HTML 태그 이전)에 한 번만 나타내야 합니다.   
<code><strong>&lt;!DOCTYPE></strong></code> 선언은 대소 문자를 구분하지 않습니다.    
<code><strong>&lt;!DOCTYPE></strong></code> HTML5 의 선언은 다음과 같습니다.

```html
<!doctype html>
```
<br>

### - Contents

####  - HTML 제목

HTML 제목은  <code><strong>&lt;h1></strong></code> ~ <code><strong>&lt;h6></strong></code> 태그 로 정의됩니다 .   
<code><strong>&lt;h1></strong></code> 은 가장 중요한 제목을 정의할 때 쓰이며, 문서에 꼭 하나 이상은 있어야 합니다.   
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

####  - HTML 단락

HTML 단락은 <code><strong>&lt;p></strong></code> 태그로 정의됩니다 .

**예)**
```html
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>
```


*****
### [목록으로 이동](README.md)
### [다음 - CSS(Cascading Style Sheet)](basic-css.md)

*****
### [홈으로 이동](https://github.com/limseongeun/frontend-knowhow)
