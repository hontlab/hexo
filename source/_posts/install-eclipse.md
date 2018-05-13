---
title: eclipse 설치 및 환경 설정 
tags: [이클립스, eclipse, 설치]
date: 2018-05-13 23:32:40
categories: setting
description: eclipse 설치 및 환경 설정 
---
{% raw %}
<ul class="order">
	<li>eclipse 설치</li>
	<li>eclipse 설정
		<ul>
			<li>memory</li>
			<li>encoding</li>
			<li>jdk</li>
			<li>tomcat</li>
			<li>browser</li>
		</ul>
	</li>
</ul>
<h2>eclipse 설치</h2>
{% endraw %}

![_1](https://user-images.githubusercontent.com/34805973/39968289-d9ba84fa-5705-11e8-821d-1a21be63be1c.PNG)

{% raw %}
<p>이클립스 사이트(<a href="https://www.eclipse.org/downloads/" target="_blank">https://www.eclipse.org/downloads/</a>) 접속하여 다운로드 패키지 버튼 클릭</p>
{% endraw %}

![_2](https://user-images.githubusercontent.com/34805973/39968290-d9e1cb64-5705-11e8-980e-bd122d4b754e.PNG)

{% raw %}
<p>우측에서 다운받고자 하는 이클립스 버전 선택</p>
{% endraw %}

![_3](https://user-images.githubusercontent.com/34805973/39968291-da098b04-5705-11e8-8d14-a189ceda8e6c.PNG)

{% raw %}
<p><span class="highlight">Eclipse IDE for Java EE Developers</span>에서 OS에 맞는 파일 다운로드</p>
{% endraw %}

![_4](https://user-images.githubusercontent.com/34805973/39968292-da3201c4-5705-11e8-810f-e315211841cf.PNG)

{% raw %}
<p>이클립스 설치 완료!</p>
<p>다운받은 이클립스 zip파일 압축 풀고, eclipse.exe 파일 실행하면 바로 이클립스 실행 가능하나 기본적인 몇가지 사항들 설정하고 사용하려고 한다.</p>
<h2>eclipse 설정</h2>
<h3>memory</h3>
{% endraw %}

![_5](https://user-images.githubusercontent.com/34805973/39968293-da5b0bfa-5705-11e8-83c7-4523374230d4.PNG)

{% raw %}
<p>위 이클립스 실행 파일이 있는 폴더에 <span class="highlight">eclipse.ini</span>라는 파일이 있는데 편집기로 열어서 보면 아래쪽에 위와 같이 표시된 부분이 보인다. <span class="highlight">이클립스 실행 시 가용할 최소메모리와 최대메모리를 설정</span>하는 부분이다.</p>
{% endraw %}

![_5_2](https://user-images.githubusercontent.com/34805973/39968367-a4dece20-5706-11e8-9b58-ee2bfae58c8e.PNG)

{% raw %}
<p>램8g 기준으로 다음과 같이 1024, 2048로 사용하는 것을 추천한다고 한다.</p>
{% endraw %}

![_6](https://user-images.githubusercontent.com/34805973/39968294-da835786-5705-11e8-8321-e1b2ba9d405d.PNG)

{% raw %}
<p>이클립스 실행하여, Windows → Preferences → General → <span class="highlight">Show heap status</span> 선택하고 저장하면 우측하단에 늘려준 힙메모리와 사용량을 확인 할 수 있다. 휴지통 버튼을 누르면 힙메모리가 비워진다.</p>
<h3>encoding</h3>
<p><span class="highlight">인코딩을 UTF-8로 바꿔주기 위한 설정</span>으로, 사전에 바꿔놓은 프로젝트 설정 자체를 export한 파일이 있어 이를 다시 import하여 사용, 이 방법이 아니라면 일일이 다 직접 바꿔야 하는 불편함이 있다.</p>
<p class="highlight">주의 할 점은 workspace가 바뀌면 다시 import해서 설정해야 한다는 것</p>
{% endraw %}

![_7](https://user-images.githubusercontent.com/34805973/39968295-daaca1e0-5705-11e8-8648-37d3671dcd7b.PNG)

{% raw %}
<p>File → Import → General → Preferences</p>
{% endraw %}

![_8](https://user-images.githubusercontent.com/34805973/39968296-dad4daf2-5705-11e8-94ad-b90bf95d4d5b.PNG)

{% raw %}
<p>초반설정 파일(초반설정.epf)을 찾은 후 Finish</p>
<p><a href="" target="_blank">초반설정 파일 다운로드</a></p>
{% endraw %}

![_9](https://user-images.githubusercontent.com/34805973/39968297-db018e26-5705-11e8-95cf-c6f122767131.PNG)

{% raw %}
<p>Windows → Preferences → encoding 검색 → 우측 파일 선택</p>
<p>이렇게 하나하나 눌러보면 다 기본 인코딩 값이 UTF-8로 바뀐 것을 확인 할 수 있다. 만약 설정파일을 import하지 않았더라면, 일일이 다 바꿨어야 하는 불편함이 여기에 있다.</p>
<h3>jdk</h3>
{% endraw %}

![_10](https://user-images.githubusercontent.com/34805973/39968298-db2a1184-5705-11e8-9b43-0cd551de4f84.PNG)

{% raw %}
<p>Windows → Preferences → java 검색 → Installed → Add → Standard VM</p>
{% endraw %}

![_11](https://user-images.githubusercontent.com/34805973/39968299-db56da98-5705-11e8-963b-429701a55d59.PNG)

{% raw %}
<p class="highlight">jdk를 설치한 경로를 지정</p>
{% endraw %}

![_12](https://user-images.githubusercontent.com/34805973/39968300-db7e6a40-5705-11e8-99b4-e9849873e824.PNG)

{% raw %}
<p class="highlight">추가한 jdk경로 체크 후 Apply 그리고 OK</p>
<h3>tomcat</h3>
{% endraw %}

![_13](https://user-images.githubusercontent.com/34805973/39968301-dba81ff2-5705-11e8-8d07-4f4986e72e1a.PNG)

{% raw %}
<p>Windows → Preferences → server 검색 → Runtime Environments → Add → 설치한 톰캣 버전 선택</p>
{% endraw %}

![_14](https://user-images.githubusercontent.com/34805973/39968302-dbed985c-5705-11e8-9122-9c992cb74c57.PNG)

{% raw %}
<p class="highlight">tomcat을 설치한 경로를 지정</p>
{% endraw %}

![_15](https://user-images.githubusercontent.com/34805973/39968303-dc1729b0-5705-11e8-92da-b9ecf39c2de2.PNG)

{% raw %}
<p>이클립스 하단 Servers 탭메뉴에서 서버 추가</p>
<p>이제 서버가 잘 추가됐는지 확인을 위해 테스트 프로젝트를 만들어보자.</p>
{% endraw %}

![_16](https://user-images.githubusercontent.com/34805973/39968304-dc4014a6-5705-11e8-9084-f228a99f06e9.PNG)

{% raw %}
<p>new → Dynamic Web Project</p>
{% endraw %}

![_17](https://user-images.githubusercontent.com/34805973/39968306-dc6908d4-5705-11e8-8888-c8e5f39005fe.PNG)

![_17_1](https://user-images.githubusercontent.com/34805973/39968307-dc9580b2-5705-11e8-9754-f3a4c2d89aeb.PNG)

{% raw %}
<p><span class="highlight">Generate web.xml 체크</span>하고 Finish</p>
{% endraw %}

![_17_2](https://user-images.githubusercontent.com/34805973/39968308-dcc0c092-5705-11e8-97af-1852f543a3e0.PNG)

{% raw %}
<p>이건 welcome-file이라 해서 기본적으로 서버 실행 후 보여줄 기본페이지를 나타내고 있다. 여기서 테스트는 이 페이지들 말고 새로 newFile.jsp를 만들어 테스트 해볼 예정</p>

<p>테스트에 앞서 아래 브라우저 설정을 통해 서버가 구동됐을 때 작동할 브라우저 선택</p>
<p>이 설정을 하지 않으면 이클립스 내부(internal) 브라우저가 작동하는데, 작업의 편의를 위해 외부(external) 브라우저 크롬으로 바꿀 생각이다.</p>

<h3>browser</h3>
{% endraw %}

![_18](https://user-images.githubusercontent.com/34805973/39968309-dcf3507a-5705-11e8-9409-9bab3b0ace60.PNG)

{% raw %}
<p>Windows → Preferences → browser 검색 → Add → 추가할 브라우저 이름과 설치경로를 지정</p>
{% endraw %}

![_19](https://user-images.githubusercontent.com/34805973/39968310-dd1a382a-5705-11e8-8308-07f141e2b4c0.PNG)

{% raw %}
<p>설치경로는 크롬에 마우스 오른쪽버튼 눌러 속성에서 대상의 내용을 가져오면 되고 <span class="highlight">앞뒤로 "는 빼야 한다.</span></p>
{% endraw %}

![_20](https://user-images.githubusercontent.com/34805973/39968311-dd457148-5705-11e8-99e3-ef3afeeef847.PNG)

{% raw %}
<p><span class="highlight">Use external web browser를 체크</span>해서 보면, 이제 <span class="highlight">크롬</span>이 브라우저 리스트에 추가된 것을 볼 수 있고 <span class="highlight">체크 후 적용해서 사용하면 된다.</span></p>
{% endraw %}

![_21](https://user-images.githubusercontent.com/34805973/39968312-dd6e4140-5705-11e8-82bb-1c8bb6075f5f.PNG)

{% raw %}
<p>이제 테스트 파일을 만들어보자.</p>
<p>webContent → new → JSP File</p>
{% endraw %}

![_22](https://user-images.githubusercontent.com/34805973/39968313-dd96048c-5705-11e8-84d9-4f53f6f20630.PNG)

{% raw %}
<p>간단히 테스트 내용을 채워넣고,</p>
{% endraw %}

![_23](https://user-images.githubusercontent.com/34805973/39968314-ddbd378c-5705-11e8-9e47-84fb4b602746.PNG)

{% raw %}
<ul>
	<li>프로젝트 선택 후 마우스 오른쪽 버튼 눌러 run누르거나,</li>
	<li>이클립스 최상단 메뉴 Run을 통하거나,</li>
	<li>Run바로 밑에 녹색 play버튼 처럼 생긴 것을 누르면</li>
</ul>
<p>톰캣 서버가 구동되고,</p>
{% endraw %}

![_24](https://user-images.githubusercontent.com/34805973/39968315-dde55802-5705-11e8-8dd2-578b4f454e18.PNG)

{% raw %}
<p>다음과 같이 url통해 접근하면 제대로 테스트 내용이 보이는 것을 확인 할 수 있다.</p>
<p>이로써, 이클립스 설치 및 설정 완료!</p>
{% endraw %}






