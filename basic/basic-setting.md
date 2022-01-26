# 개발 환경 셋팅

웹페이지 제작을 하기 위해서는 가장 먼저 개발 환경이 셋팅이 되어야 시작을 할 수 있습니다. 코딩을 하기 위한 **제작 툴**,  코딩한 결과 화면을 확인하기 위한 **웹 브라우저**, 소스 관리를 하기 위한 **버전 관리 툴**, 웹서버에 파일을 업로드 할 **파일전송 프로토콜(FTP) 프로그램**이 셋팅 돼 있어야 합니다. 현재 제가 작업 시에 셋팅 한 기준으로 소개를 하는 것이니, 관련된 다른 툴을 사용해도 무관합니다.

* <a href="#제작툴">**제작 툴**(Code&amp;Image Editor)</a>
* <a href="#웹브라우저">**웹 브라우저**(Web Browser)</a>
* <a href="#버전관리툴">**버전 관리 툴**(Version Control)</a>
* <a href="#ftp">**파일 전송 프로토콜**(FTP) **프로그램**</a>

----

## 제작 툴(Code&amp;Image Editor) <a id="제작툴"></a>

코딩을 하기 위해서 필요한 제작 툴에는 크게 **코딩 툴**과 **이미지 편집 툴**이 있습니다. 

### - 코딩 툴

우선 웹페이지를 제작할 때 사용하는 코딩 툴로는 여러가지가 있지만, 지금 현재 제가 사용하는 툴은 **'비주얼스튜디오( VisualStudio )'** 와 **'에디트플러스(EditPlus)'** 가 있습니다. 직장에서는 라이센스가 필요한 에디트플러스를 사용하고, 개인 소스 작업을 할 때에는 주로 비주얼스튜디오를 사용하고 있습니다. 에디터는 각각 장단점이 있기 때문에 작업할 때 개인마다 사용하기 편한 것으로 선택해서 사용하시면 됩니다. ( <a rel="noreferrer noopener" href="https://m.blog.naver.com/cronix7601/222038061002" target="_blank">HTML 에디터 종류 바로가기</a>)   
또한 최근에는 **<a href="https://codepen.io/" target="_blank" rel="noreferrer noopener">'Codepen'</a>**, **<a rel="noreferrer noopener" href="https://codesandbox.io/" target="_blank">'CodeSandbox'</a>** 와 같은 온라인 제작 툴도 잘 돼 있어 연습 시에 활용하면 유용합니다.

* 비주얼스튜디오 - <a rel="noreferrer noopener" href="https://code.visualstudio.com/?wt.mc_id=vscom_downloads" target="_blank">다운로드</a>, <a rel="noreferrer noopener" href="https://demun.github.io/vscode-tutorial/" data-type="URL" data-id="https://demun.github.io/vscode-tutorial/" target="_blank">사용설명</a>

<img width="360" src="https://user-images.githubusercontent.com/13953651/150911614-86dd6929-788e-4032-8704-25d4b31e3bdf.png" alt="" >

* 에디트플러스 - <a rel="noreferrer noopener" href="https://www.editplus.com/kr/download.html" target="_blank">다운로드</a>, <a rel="noreferrer noopener" href="https://itgroovy.tistory.com/1009" target="_blank">사용설명</a>

<img width="360" src="https://user-images.githubusercontent.com/13953651/150911817-f6d6dd73-683e-4a27-9c7a-8cede0b8b5d3.png" alt="" >

<br >

### - 이미지 편집 툴 ###

프로젝트를 진행 할 시에 디자이너에게 디자인 된 시안을 전달 받으면, 프론트엔드 개발자는 코딩에 필요한 이미지를 잘라서 사용해야 하는데 이 때 사용하는 툴이 이미지 편집 툴입니다. 대부분 시안이 **Adobe Photoshop**을 사용하여 PSD 파일로 전달 되기에, 시안을 확인하고 편집하기 위해서는 설치를 해 주어야 합니다. 최근에는 Adobe사에서 클라우드 기반으로 서비스를 하기 때문에 시안의 최종 형태를 확인해서 버전에 맞는 프로그램을 준비해서 사용해야 합니다.

* 포토샵 - <a rel="noreferrer noopener" href="https://www.adobe.com/kr/products/photoshop.html" target="_blank">다운로드</a>, <a rel="noreferrer noopener" href="https://blog.naver.com/hyoyeol/70141433837" target="_blank">이미지 자르기 설명</a>

<img width="360" src="https://user-images.githubusercontent.com/13953651/150913291-2ef9a0bb-c19e-4953-8207-457322264c55.png" alt="" >

또한 PSD를 온라인으로도 편집이 가능하도록 서비스하고 있는 사이트가 있습니다. <a rel="noreferrer noopener" href="https://www.photopea.com/" target="_blank">**'Photopea'**</a> 라는 사이트인데, 인터페이스가 거의 포토샵과 흡사하기에 사용하기에 거부감이 없고 편리합니다.

<img width="360" src="https://user-images.githubusercontent.com/13953651/150913396-2e4abe2c-c3d2-4311-a6ff-ce36e0a33b03.png" alt="" >

<br >

## 웹 브라우저(Web Browser) <a id="웹브라우저"></a>

제작 툴을 사용하여 코딩한 결과물을 확인하기 위해서는 **웹 브라우저**가 필요합니다. 웹 브라우저의 종류에는 여러가지가 있으며, 그 가운데 작업 시에 가장 많이 사용하는 웹 브라우저는 **구글의 크롬 브라우저(Google Chrome )** 입니다.   
크롬 브라우저는 가장 대중화 된 브라우저이고, 개발자 도구(F12)를 통해 소스 확인은 물론이고, 에디터처럼 실시간 소소 수정을 하면서 화면 확인도 할 수 있고, 모바일 환경에서의 화면도 설정(Toggle device toolbar)을 통해 확인할 수 있는 기능들이 있어 유용합니다. 많은 사람들이 여러 웹 환경에서 웹을 이용하기에 한 브라우저에서만 확인을 하면 안되고 '**크로스브라우징**- _작업 소스가 여러 브라우저에서 똑같은 화면으로 보여지게 하는 코딩 방식_' 이 중요하기에 최소한 3개 이상의 다른 웹 브라우저에서도 확인이 필요합니다.   
우리나라에서는 인터넷 익스플로러 브라우저를 많이 사용하기에 버전별 확인이 필요하며, 그 밖에도  모질라 파이어폭스(Mozilla Firefox), 마이크로소프트 엣지(Microsoft Edge), 오페라(Opera), 사파리(Safari) 등이 있습니다. 웹 브라우저는 각 해당 사이트에서 다운로드 하시면 됩니다.

| 웹 브라우저 | 링크 |
|:---:|:---:|
| <img style="width: 100px;" src="https://github.com/limseongeun/frontend-knowhow/blob/main/basic/images/img_chrome.png" alt=""><br>구글 크롬 | <a rel="noreferrer noopener" href="https://www.google.co.kr/chrome/?brand=IBEF&amp;gclid=Cj0KCQjwwY-LBhD6ARIsACvT72PaNyeczLM8oFkkTePaRVXAqJVVsgw0aE3U1F-BDV9eOExoJE1zPr4aAlTeEALw_wcB&amp;gclsrc=aw.ds" target="_blank">다운로드 바로가기</a> |
| <img style="width: 100px;" src="https://github.com/limseongeun/frontend-knowhow/blob/main/basic/images/img_ie.png" alt=""><br>인터넷 익스플로러 | <a rel="noreferrer noopener" href="https://support.microsoft.com/ko-kr/windows/internet-explorer-%EB%8B%A4%EC%9A%B4%EB%A1%9C%EB%93%9C%ED%95%98%EA%B8%B0-d49e1f0d-571c-9a7b-d97e-be248806ca70#ID0EBBD=Windows_10" target="_blank">다운로드 바로가기</a> |
| <img style="width: 100px;" src="https://github.com/limseongeun/frontend-knowhow/blob/main/basic/images/img_edge.png" alt=""><br>마이크로소프트 엣지 | <a rel="noreferrer noopener" href="https://www.microsoft.com/ko-kr/edge" target="_blank">다운로드 바로가기</a> |
| <img style="width: 100px;" src="https://github.com/limseongeun/frontend-knowhow/blob/main/basic/images/img_fx.png" alt=""><br>모질라 파이어폭스 | <a rel="noreferrer noopener" href="https://www.mozilla.org/ko/firefox/new/" target="_blank">다운로드 바로가기</a> |
| <img style="width: 100px;" src="https://github.com/limseongeun/frontend-knowhow/blob/main/basic/images/img_sa.png" alt=""><br>애플 사파리 | <a rel="noreferrer noopener" href="https://safari.softonic.kr/" target="_blank">다운로드 바로가기</a> |
| <img style="width: 100px;" src="https://github.com/limseongeun/frontend-knowhow/blob/main/basic/images/img_op.png" alt=""><br>오페라 | <a rel="noreferrer noopener" href="https://www.opera.com/ko/computer/opera?utm_campaign=%2300%20-%20WW%20-%20Search%20-%20EN%20-%20Branded&amp;gclid=Cj0KCQjwwY-LBhD6ARIsACvT72Mx8vCLe0yMswSS7Ed5tdjVY_7UbKx0I7leYve3ympf-XkNHF9dYwYaAupaEALw_wcB" target="_blank">다운로드 바로가기</a> |
| <img style="width: 100px;" src="https://github.com/limseongeun/frontend-knowhow/blob/main/basic/images/img_whale.png" alt=""><br>네이버 웨일 | <a rel="noreferrer noopener" href="https://whale.naver.com/" target="_blank">다운로드 바로가기</a> |

<br >

## 버전 관리 툴(Version Control) <a id="버전관리툴"></a>

작업한 소스를 버전별로 관리해 주는 툴을 활용하면 좋습니다. 개인작업뿐만 아니라 팀단위 프로젝트를 진행할 때 더욱 필요합니다. 작업자가 서로 같은 소스를 수정하다가 소스가 꼬일 경우 잘못될 수가 있는데, 버전 관리 툴을 사용하면 이같은 문제를 방지할 수 있습니다. 보편적으로 가장 많이 사용하는 툴로는 깃(Git), 깃허브(Github) 비트버켓(Bitbucket), TortoiseSVN 등이 있습니다.

* 깃(Git)/깃허브(Github) - <a rel="noreferrer noopener" href="https://git-scm.com/downloads" target="_blank">다운로드</a>, <a rel="noreferrer noopener" href="https://rogerdudler.github.io/git-guide/index.ko.html" target="_blank">사용설명</a>, <a rel="noreferrer noopener" href="https://nevertrustbrutus.tistory.com/m/153" target="_blank">깃허브 같이 사용하기</a>

<img width="360" src="https://user-images.githubusercontent.com/13953651/150916607-e07bc3d3-dbf1-4141-a202-306f71aa9765.png" alt="" >

* 비트버켓(Bitbucket) - <a rel="noreferrer noopener" href="https://devkoboso.com/308" target="_blank">사용설명</a>

<img width="360" src="https://user-images.githubusercontent.com/13953651/150916777-4ae675f2-bfe0-498e-90f4-c69263adb9db.png" alt="" >

* TortoiseSVN - <a rel="noreferrer noopener" href="https://tortoisesvn.net/downloads.html" target="_blank">다운로드</a>, <a rel="noreferrer noopener" href="https://webobj.tistory.com/47" target="_blank">사용설명</a>

<img width="360" src="https://user-images.githubusercontent.com/13953651/150916915-3a3daf84-a816-498a-bd89-9406971c0bc8.png" alt="" >

<br >

## 파일 전송 프로토콜(FTP) 프로그램 <a id="ftp"></a>

자신의 컴퓨터(Local)에서 최종 작업한 소스를 서버에 전송해야 실제 인터넷상에서 웹서비스를 이용할 수 있습니다. 이 때 주로 사용하는 파일 전송 프로토콜(File Transfer Protocol) 프로그램으로는 **'파일질라(FileZilla)'** 가 있습니다. 파일질라를 설치하고 전송할 서버(사전에 구축한 웹호스팅)의 접속정보인 호스트, 사용자명, 비밀번호, 포트 등을 입력해야 접속 할 수 있습니다. 서버에 접속이 되면 작업한 파일을 자신의 컴퓨터에서 FTP 서버로 업로드를 시키면 됩니다.

* 파일질라 - <a rel="noreferrer noopener" href="https://filezilla.softonic.kr/download" target="_blank">다운로드</a>, <a rel="noreferrer noopener" href="https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&amp;blogId=anysecure3&amp;logNo=220682941990" target="_blank">사용설명</a>

<img width="360" src="https://user-images.githubusercontent.com/13953651/150917091-f7645704-3a24-45b1-b0e8-5d8887b7274f.png" alt="" >

*****
### [목록으로 이동](README.md)
### [다음 - HTML(HyperText Markup Language)](basic-html.md)

*****
### [홈으로 이동](https://github.com/limseongeun/frontend-knowhow)
