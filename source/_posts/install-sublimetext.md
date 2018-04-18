---
title: 서브라임텍스트3 설치 및 설정
tags: [서브라임텍스트3, sublimetext3, 플러그인, 설치, 설정]
date: 2018-04-17 09:40:29
categories: 설치
description:
---
{% raw %}

<h2>설치</h2>
<p>서브라임텍스트는 html, css, 스크립트 등 화면단을 구성할 때 쓰기 편하고 가벼운 툴로써 다양한 단축키 지원 및 태그별 색상이 구분돼 시안성이 좋고, 게다가 무료이기 때문에 많이 사용한다. 아래 링크에서 OS에 맞게 다운로드 받으면 된다. 특별한 부분 없이 next 눌러 설치하면 된다.</p>
<p><a href="https://www.sublimetext.com/3" target="_blank">서브라임텍스트3 다운로드</a></p>
{% endraw %}

![_0](https://user-images.githubusercontent.com/34805973/38842714-756a00aa-4226-11e8-99e1-c275fb52fb22.PNG)


{% raw %}


<h2>설정</h2>
<h3>1. 플러그인 설정</h3>
<p>일단 서브라임텍스트를 다운받아 설치하였다면, 더 편리하게 사용하기 위해 플러그인을 설치해 사용하는 것이 일반적이다. 그런데 여기서 특이한 것이 아래와 같이 <span class="highlight">서브라임텍스트에서 따로 명령어처럼 입력해 플러그인을 설치</span>한다는 것인데,</p>
{% endraw %}

![_2](https://user-images.githubusercontent.com/34805973/38842612-f452dc3a-4225-11e8-883b-696623657244.PNG)

{% raw %}

<p>하단의 창을 어떻게 띄우고 어떤 명령어를 입력하는지에 대한 사항은 아래와 같고,</p>
{% endraw %}

![_1](https://user-images.githubusercontent.com/34805973/38842929-ad2e4fea-4227-11e8-9b9b-65f604330b46.PNG)

{% raw %}

<p><a href="https://packagecontrol.io/installation#st3" target="_blank">서브라임텍스트 버전별 플러그인 설치 코드(명령어)</a> 이곳에서 복사해서 붙여 넣으면 된다. 위에서 봤던 하단의 창에 붙여넣은 후 엔터를 치면, 아래와 같이 플러그인을 세팅 할 수 있는 환경(패키지)이 구성된 것이다.</p>
{% endraw %}

![_3](https://user-images.githubusercontent.com/34805973/38843008-103de5fa-4228-11e8-9659-19ee1d574ff4.PNG)


{% raw %}

<p>이제 본격적으로 상단의 창을 띄어 플러그인을 설치할 차례인데, 상단의 창을 띄우는 방법은 ctrl+shift+p를 누르면 되고, install이라고 검색하면 Package Controll:Install Package가 나오게 된다. 가끔(?) 검색되지 않는 경우도 있는데 서브라임텍스트를 재실행해보고 이래도 안되면, 패키지 구성(설치)이 잘 안된 것이다...ㅠㅠ 그럼 이어나가서 위에서 install을 검색하고 엔터를 치고 조금 기다리면 아래처럼 플러그인을 검색해서 설치할 수 있는 창이 나오고 검색해서 해당 플러그인을 설치하면 된다.</p>
{% endraw %}

![_8](https://user-images.githubusercontent.com/34805973/38843554-7fab3904-422a-11e8-94b4-5f51c0619f03.png)

![_6](https://user-images.githubusercontent.com/34805973/38843495-2c3d1990-422a-11e8-90a4-8c48bbdf3d54.png)

![_7](https://user-images.githubusercontent.com/34805973/38843464-056d14fa-422a-11e8-84a8-796c5f13545e.png)


{% raw %}

<p>플러그인 설치에 성공하면, 위와 같이 설치가 완료됐다는 창이 띄고 내가 설치한 플러그인을 확인하려면 Preferences > Package Settings 메뉴를 확인하면 된다.</p>
{% endraw %}

![_5](https://user-images.githubusercontent.com/34805973/38843355-9c7a3b44-4229-11e8-9240-504783c108cb.png)

{% raw %}

<p>위는 개인적으로 화면단 작업 시 주요하게 썼던 플러그인으로,</p>
<ul>
	<li>Bracket Highlighter
		<p>{},[],"",'',() 와 같이 열리고 닫히는 기호가 쌍으로 존재해야 하는 코드를 하이라이트처리해주는 확장기능</p>
	</li>
	<li>Emmet
		<p>일명 Zen Coding이라 불리는 html코드 작성의 생산성을 높여주는 기술로 div*5 처럼 특정 문법에 맞게 작성하고 탭키를 누르면 div가 5개 자동생성 된다든지 하는 경우이다.</p>
	</li>
	<li>Side Bar(플러그인 검색 시에는 SideBarEnhancement로 나오는데 이걸 받으면 된다.)
		<p>서브라임텍스트 작업창 좌측에 작업 파일 폴더구조를 나타내는 화면을 띄울 때(View > Side Bar > Show Open Files 메뉴), 폴더구조를 보다 더 명확히 구분돼 보여주는 기능</p>
	</li>
	<li>TortoiseSVN
		<p>일명 거북이로 불리는 TortoiseSVN을 설치하여 서브라임텍스트 툴에서 바로 형상관리 가능</p>
	</li>
	<li>ConvertToUTF8
		<p>인코딩 설정을 자동으로 UTF-8로 맞춰준다.</p>
	</li>
</ul>

<p class="highlight">여기서 주의할 점은, 플러그인을 설치할 때마다 ctrl+shift+p를 눌러 install이라고 검색한 후 Package Controll:Install Package가 나온 상태에서 검색해야 한다는 것이다.</p>

<h3>2. 유저세팅(font, 크기, 미니맵 등 실제 서브라임텍스트 작업창 스타일) 설정</h3>
<p>Preferences > Settings를 누르면 새로운 창에 하나 띄워지고, 여기에 아래 내용을 전체선택 복사 붙여 넣고 덮어써 저장한다.</p>
<p>추가적으로, 코딩 시 가독성 좋은 <a href="https://github.com/naver/d2codingfont" target="_blank">d2coding폰트 다운로드</a></p>
{% endraw %}

![_9](https://user-images.githubusercontent.com/34805973/38844818-10f8a4be-4230-11e8-81a8-d7f412ae35b6.png)


{% raw %}
<pre>
	{
		"always_show_minimap_viewport": true,
		"bold_folder_labels": true,
		"caret_style": "smooth",
		"draw_minimap_border": true,
		"fade_fold_buttons": false,
		"font_face": "d2coding",
		"font_size": 13,
		"highlight_modified_tabs": true,
		"ignored_packages":
		[
			"Vintage"
		],
		"line_padding_bottom": 1,
		"line_padding_top": 1,
		"tab_size": 3,
		"word_wrap": true
	}
</pre>

<h3>3. 키바인딩(단축키) 설정</h3>
<p>Preferences > Key Bindings를 누르면 새로운 창에 하나 띄워지고, 여기에 아래 내용을 전체선택 복사 붙여 넣고 덮어써 저장한다.</p>
<p>블럭지정하거나 하지 않고 "ctrl+shift+r" 단축키를 눌러 코드를 정렬하는 기능이다.</p>
{% endraw %}

![_10](https://user-images.githubusercontent.com/34805973/38844839-1ce7d344-4230-11e8-950a-26c34ef34c88.png)


{% raw %}
<pre>
[
{ "keys": ["ctrl+shift+r"], "command": "reindent" , "args": { "single_line": false } }
]
</pre>
{% endraw %}