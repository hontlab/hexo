---
title: Tomcat 설치 및 환경변수 설정
tags: [tomcat, 톰캣, 설치, 환경변수, 설정]
date: 2018-05-13 19:18:44
categories: setting
description: Tomcat 설치 및 환경변수 설정
---
{% raw %}
<ul class="order">
	<li>Tomcat 설치</li>
	<li>Tomcat 환경변수 설정
		<ul>
			<li>CATALINA_HOME</li>
			<li>CLASSPATH</li>
		</ul>
	</li>
</ul>
<h2>Tomcat 설치</h2>

{% endraw %}

![_1](https://user-images.githubusercontent.com/34805973/39966202-a4d5bfa2-56e2-11e8-8ef9-4d5177e73904.PNG)


{% raw %}
<p>아파치 사이트(<a href="http://tomcat.apache.org/" target="_blank">http://tomcat.apache.org/</a>) 접속하여 맨 하단 Tomcat 클릭</p>
{% endraw %}

![_2](https://user-images.githubusercontent.com/34805973/39966203-a50341ca-56e2-11e8-929f-d8b1b8c2313a.PNG)

{% raw %}
<p>해당하는 파일 다운로드 후 zip파일 압축 푼다.</p>
{% endraw %}

![_3](https://user-images.githubusercontent.com/34805973/39966204-a52e3c68-56e2-11e8-9337-33ffe51e5ba9.PNG)

![_4](https://user-images.githubusercontent.com/34805973/39966205-a5616214-56e2-11e8-8400-ad0fdb86744c.PNG)

{% raw %}
<p>해당 경로(conf 폴더) 이동하여 <span class="highlight">server.xml</span>을 열어보면 다음과 같이 포트번호가 8080으로 돼있는 것을 확인할 수 있다. 그런데 <span class="highlight">포트번호 8080은 오라클에서 사용하기 때문에 충돌 가능성 때문에, 아래와 같이 80(http포트)으로 바꿔준다.</span></p>
{% endraw %}

![_4_2](https://user-images.githubusercontent.com/34805973/39966206-a58f494a-56e2-11e8-9ec6-e94188b34a0f.PNG)

{% raw %}
<p>이제는 톰캣이 정상적으로 작동하는 지 확인해보려고 하는데 그 방법은 아래와 같다.</p>
{% endraw %}

![_5](https://user-images.githubusercontent.com/34805973/39966207-a5bed318-56e2-11e8-9f4e-63969c32659d.PNG)

{% raw %}
<p>해당경로(bin폴더)에서 <span class="highlight">startup.bat</span>이라는 배치파일(MS-DOS, OS/2, 윈도우에서 쓰이는 배치 파일(batch file)은 명령 인터프리터에 의해 실행되게끔 고안된 명령어들이 나열되어 있는 텍스트 파일이다.) 더블클릭 하면,</p>
{% endraw %}
![_6](https://user-images.githubusercontent.com/34805973/39966208-a5eb8534-56e2-11e8-93f8-a17e595e02f1.PNG)

{% raw %}
<p>위와 같이 배치파일이 실행되는데 실행창에서 오류나 심각 메시지가 나오지 않는지 확인한다.</p>
{% endraw %}

![_7](https://user-images.githubusercontent.com/34805973/39966209-a62b331e-56e2-11e8-8d18-7c332479c866.PNG)

{% raw %}
<p>이렇게 톰캣 서버 실행 후, 브라우저 주소창에 <span class="highlight">localhost</span>를 입력하여 <span class="highlight">톰캣 고양이 화면이 나오면 성공!(서버가 제대로 돌고 있다는 것)</span></p>
{% endraw %}

![_8](https://user-images.githubusercontent.com/34805973/39966210-a66acac4-56e2-11e8-8ee5-12e3e191109f.PNG)

{% raw %}
<p>톰캣 종료는 <span class="highlight">shutdown.bat</span> 배치파일 더블클릭</p>

<h2>Tomcat 환경변수 설정</h2>
<h3>CATALINA_HOME</h3>
{% endraw %}

![_9](https://user-images.githubusercontent.com/34805973/39966211-a6aa6698-56e2-11e8-9beb-ae1a8cc49377.PNG)

{% raw %}
<p>변수 이름 : CATALINA_HOME <br> 변수 값 : 톰캣 설치 경로</p>
{% endraw %}

![_10](https://user-images.githubusercontent.com/34805973/39966212-a6d35a94-56e2-11e8-990c-3be0d56d191e.PNG)

{% raw %}
<p>jdk 설치한 후 jdk 환경변수 설정했다면, 이미 CLASSPATH가 환경변수로 잡혀 있을텐데 그러면 수정 눌러서 다음과 같이 수정 혹은 추가 해준다.</p>
<p>변수 이름 : CLASSPATH <br> 변수 값 : %JAVA_HOME%\jre\lib\rt.jar;%CATALINA_HOME%\lib\servlet-api.jar</p>
<p>복사해서 붙여 넣으면 \이 아니라 위처럼 나온다.</p>
<ul>
	<li>rt.jar는 lang패키지 클래스, rmi 클래스, 컬렉션 클래스 등 모두 갖고 있는 클래스 압축파일</li>
	<li>servlet-api.jar는 어플리케이션 서버(확장된 CGI)를 실행하기 위한 서블릿 클래스 등을 갖고 있는 클래스 압축파일</li>
</ul>
{% endraw %}

![_11](https://user-images.githubusercontent.com/34805973/39966408-3ac1daf2-56e6-11e8-8398-f495e06caf5e.PNG)






