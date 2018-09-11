---
title: JDK 설치 및 환경변수 설정
tags: [jdk, 설치, 환경변수, 설정]
date: 2018-05-13 15:13:26
categories: setting
description: JDK 설치 및 환경변수 설정
---
{% raw %}

<ul class="order">
	<li>JDK 설치</li>
	<li>JDK 환경변수 설정
		<ul>
			<li>JAVA_HOME</li>
			<li>Path</li>
			<li>CLASSPATH</li>
		</ul>
	</li>
</ul>

{% endraw %}

{% raw %}
<h2>JDK 설치</h2>
{% endraw %}

![jdk _1](https://user-images.githubusercontent.com/34805973/39964487-b20d2060-56c0-11e8-9c29-92f7301a612f.PNG)

{% raw %}
오라클 사이트(<a href="https://www.oracle.com/index.html" target="_blank">https://www.oracle.com/index.html</a>) 접속하여 다운로드 버튼 클릭
{% endraw %}

![jdk _2](https://user-images.githubusercontent.com/34805973/39964488-b246c02c-56c0-11e8-8a4f-1dd3cd8b34f7.PNG)



![jdk _3](https://user-images.githubusercontent.com/34805973/39964489-b2746888-56c0-11e8-8b8a-81cb1f67b79f.PNG)

{% raw %}
<p>Java SE(Standard Edition) 버전 선택, EE(Enterprise Edition)는 자바를 이용한 서버측 개발을 위한 플랫폼이라 합니다.</p>
<p>위 페이지에서 맨 아래로 이동하면 jdk 이전버전이 다운 가능합니다(여기서는 jdk 1.7버전을 다운)</p>
{% endraw %}

![jdk _4](https://user-images.githubusercontent.com/34805973/39964490-b29fb128-56c0-11e8-9820-5012f5bb912c.PNG)

![jdk _5](https://user-images.githubusercontent.com/34805973/39964491-b2c6a40e-56c0-11e8-9e3e-9bf6b99383a3.PNG)

{% raw %}
<p>여기까지 오는 링크(<a href="http://www.oracle.com/technetwork/java/javase/archive-139210.html" target="_blank">http://www.oracle.com/technetwork/java/javase/archive-139210.html</a>)</p>
{% endraw %}

![jdk _6](https://user-images.githubusercontent.com/34805973/39964492-b301d7ae-56c0-11e8-9a1a-c246394bc7e9.PNG)

{% raw %}
<p>해당 OS와 비트에 맞는 파일 다운로드(윈도우 64비트라면 위 표시된 파일 다운로드)</p>
{% endraw %}

![jdk _7](https://user-images.githubusercontent.com/34805973/39964494-b3493c34-56c0-11e8-9dde-68c77ef68443.PNG)

{% raw %}
<p>일단 jdk는 설치완료!</p>
{% endraw %}

![jdk _8](https://user-images.githubusercontent.com/34805973/39964495-b3747f84-56c0-11e8-98a2-4d44fa82ad56.PNG)


{% raw %}
<p>명령 프롬프트(CMD)에서 설치된 자바 버전 확인(명령어 <span class="highlight">java -version</span>)</p>
<p>자바 컴파일러 버전 확인(명령어 <span class="highlight">javac -version</span>) 하려고 했는데 다음과 같이 실행 불가</p>
<p>jdk 설치에서 끝나는 것이 아니라 환경변수 설정을 해줘야 합니다.</p>

<h2>JDK 환경변수 설정</h2>
<p>환경 변수는 말 그대로 변수에 어떤 값을 저장시키고 이를 환경에 저장하는 것, 환경에 저장한다는 말은 그 환경 내의 <span class="highlight">모든 프로그램이 그 변수의 값을 알 수 있게 된다는 뜻</span>, 그러니까 OS와 jdk를 이용하는 모든 프로그램에 jdk가 설치됐다고 알려주는 것으로 일단 이해했습니다.</p>
<p><span class="highlight">3가지 환경변수를 설정</span>해야 하는데 다음과 같습니다.</p>
<ul>
	<li>첫번째 환경변수, <span class="highlight">JAVA_HOME</span>(뒤이어 설정할 환경변수를 보다 편하게 설정하도록 변수화)</li>
	<li>두번째 환경변수, <span class="highlight">Path</span>(어느 위치에서도 자바 컴파일(javac) 및 실행(java) 명령어 사용 가능하도록)</li>
	<li>세번째 환경변수, <span class="highlight">CLASSPATH</span>(컴파일에 필요한 필수 클래스 로드하도록)</li>
</ul>

<h3>JAVA_HOME 설정</h3>
<p class="highlight">뒤이어 설정할 환경변수를 보다 편하게 설정하도록 변수화</p>
{% endraw %}

![jdk _9](https://user-images.githubusercontent.com/34805973/39964496-b3a9c356-56c0-11e8-8deb-1461f845d617.PNG)

{% raw %}
<p>내 PC 마우스 오른쪽 버튼 → 속성</p>
{% endraw %}

![jdk _10](https://user-images.githubusercontent.com/34805973/39964497-b3d64b92-56c0-11e8-8d2a-a8fcca608c62.PNG)

{% raw %}
<p>고급 시스템 설정 → 환경 변수 → <span class="highlight">시스템 변수</span>(주의! 위의 사용자 변수가 아니라 아래 시스템 변수입니다.) → 새로 만들기</p>
{% endraw %}

![jdk _11](https://user-images.githubusercontent.com/34805973/39964498-b4069bb2-56c0-11e8-8962-57ee266006f6.PNG)

{% raw %}
<p>변수 이름 : JAVA_HOME <br> 변수 값 : jdk 설치 경로</p>

<h3>Path 설정</h3>
<p class="highlight">어느 위치에서도 자바 컴파일(javac) 및 실행(java) 명령어 사용 가능하도록</p>
{% endraw %}

![jdk _12](https://user-images.githubusercontent.com/34805973/39964499-b432782c-56c0-11e8-8d19-14b53a8fd011.PNG)

{% raw %}
<p>Path 환경변수의 경우 이미 있습니다. 따라서 선택 후 편집을 누릅니다.</p>
<p>그리고 창이 뜨면 새로 만들기</p>
{% endraw %}

![jdk _13](https://user-images.githubusercontent.com/34805973/39964500-b45ee74a-56c0-11e8-8b9c-75a455ffcddf.PNG)

{% raw %}
<p>%JAVA_HOME%\bin</p>
<p>복사 후 붙여 넣으면 \가 아니라 위처럼 표시됩니다.</p>
<h3>CLASSPATH</h3>
<p class="highlight">컴파일에 필요한 필수 클래스 로드하도록</p>
{% endraw %}

![jdk _14](https://user-images.githubusercontent.com/34805973/39964501-b48afec0-56c0-11e8-874d-9aab103b6bd8.PNG)

{% raw %}
<p>변수 이름 : CLASSPATH <br> 변수 값 : %JAVA_HOME%\bin</p>
<p>이제 3가지 환경변수 설정 모두 끝!</p>
{% endraw %}

![jdk _15](https://user-images.githubusercontent.com/34805973/39964502-b4cacea6-56c0-11e8-8a6b-7b3debce1926.PNG)

{% raw %}
<p>다시 한번, CMD에서 자바 컴파일 버전 확인(<span class="highlight">javac -version</span>)을 해보면 이제 잘 나오는 것을 확인할 수 있습니다.</p>
{% endraw %}

