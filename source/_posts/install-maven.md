---
title: Maven 설치 및 환경 설정
tags: [Maven, 메이븐, 설치, 설정]
date: 2018-05-14 10:18:45
categories: setting
description: Maven 설치 및 환경 설정
---
{% raw %}
<ul class="order">
	<li>Maven 설치</li>
	<li>Maven 설정
		<ul>
			<li>환경변수 설정</li>
			<li>이클립스 설정
				<ul>
					<li>Maven 연결</li>
					<li>Maven 로컬저장소 지정</li>
					<li>Maven target 폴더 제외</li>
				</ul>
			</li>
		</ul>
	</li>
</ul>
<h2>Maven 설치</h2>
{% endraw %}

![_1](https://user-images.githubusercontent.com/34805973/39973945-23ccbee6-5760-11e8-9406-0de416ff6def.PNG)

![_2](https://user-images.githubusercontent.com/34805973/39973946-23f8e264-5760-11e8-9550-0c3154c0c9ad.PNG)

{% raw %}
<p>Maven 사이트(<a href="https://Maven.apache.org/" target="_blank">https://Maven.apache.org/</a>) 접속하여 파일 다운로드 후 zip파일 압축 풀기</p>
<h2>Maven 설정</h2>
<h3>환경변수 설정</h3>
{% endraw %}

![_3](https://user-images.githubusercontent.com/34805973/39973947-2437b37c-5760-11e8-811f-8ceb83eac3be.PNG)

{% raw %}
<p>변수 이름 : <span class="highlight">MAVEN_HOME</span> <br> 변수 값 : Maven 설치 경로</p>
{% endraw %}

![_4](https://user-images.githubusercontent.com/34805973/39973948-2462fa28-5760-11e8-92f7-5067f1ce186a.PNG)

{% raw %}
<p>Path 환경변수 편집 누르고 새로 만들기해서 <span class="highlight">%MAVEN_HOME%\bin</span></p>
<p>\ 부분은 복사 붙여넣기 하면 위 화면 처럼 제대로 나온다.</p>
{% endraw %}

![_5](https://user-images.githubusercontent.com/34805973/39973949-248f36b0-5760-11e8-84e5-9e51c7cb70ce.PNG)

{% raw %}
<p>CMD에서 Maven 버전 확인 명령어(<span class="highlight">mvn -version</span>)를 실행하여 제대로 설치됐는지 확인</p>
<h3>이클립스 설정</h3>
<h4>Maven 연결</h4>
{% endraw %}

![_6](https://user-images.githubusercontent.com/34805973/39973950-24bf10ce-5760-11e8-8459-7c5101d2640a.PNG)

{% raw %}
<p>Windows → Preferences → Maven 검색 → Installations → Add</p>
{% endraw %}

![_7](https://user-images.githubusercontent.com/34805973/39973951-24e8e7a0-5760-11e8-82d0-41d6c9659476.PNG)

{% raw %}
<p>Maven 설치 경로 추가</p>
{% endraw %}

![_8](https://user-images.githubusercontent.com/34805973/39973952-25124da2-5760-11e8-8f33-fbae499a8939.PNG)

{% raw %}
<p>체크 후 OK</p>
<h4>Maven 로컬저장소 지정</h4>
{% endraw %}

![_9](https://user-images.githubusercontent.com/34805973/39973953-253df1e6-5760-11e8-9649-510b18054541.PNG)

{% raw %}
<p>다시 Windows → Preferences → Maven 검색 → User Settings → <span class="highlight">Maven 설치 경로 conf 폴더 setting.xml 파일 선택</span></p>
{% endraw %}

![_10](https://user-images.githubusercontent.com/34805973/39973954-2569b876-5760-11e8-927c-c9881ed76b9e.PNG)

{% raw %}
<p>Maven 설치경로에 <span class="highlight">repository 라는 폴더 생성</span></p>
{% endraw %}

![_11](https://user-images.githubusercontent.com/34805973/39973955-259452ac-5760-11e8-9cb9-adce3ca8471b.PNG)

{% raw %}
<p>다시 돌아와 open file 버튼 클릭</p>
{% endraw %}

![_12](https://user-images.githubusercontent.com/34805973/39973956-25c02850-5760-11e8-801e-77c155b4598d.PNG)

{% raw %}
<p>setting.xml 파일이 열리고 아래 Source탭을 누른다.</p>
{% endraw %}

![_13](https://user-images.githubusercontent.com/34805973/39973957-25eb8dc4-5760-11e8-953f-e194fdc77180.PNG)

![_14](https://user-images.githubusercontent.com/34805973/39973958-261b2a0c-5760-11e8-8d3f-705caec54dae.PNG)

{% raw %}
<p>빨간 박스 부분을 <span class="highlight">&lt;localRepository&gt; repository 폴더 경로 &lt;/localRepository&gt;</span></p>
<p>이제 Maven이 이클립스에 잘 설정됐는 지 확인하는 방법으로 아래와 같다.</p>
{% endraw %}

![_15](https://user-images.githubusercontent.com/34805973/39973959-26465b14-5760-11e8-8045-9cfa3812ecba.PNG)

![_16](https://user-images.githubusercontent.com/34805973/39973960-2672e3e6-5760-11e8-8b11-621eaf941b3b.PNG)

{% raw %}
<p>Windows → Show View → Other → Maven 검색 후 Maven Repositories 선택</p>
{% endraw %}

![_17](https://user-images.githubusercontent.com/34805973/39973961-269f6bf0-5760-11e8-8ce6-389c37e9e6cb.PNG)

{% raw %}
<p>이클립스 하단 Maven Repositories 탭 → Local Repositories → Local Repository 부분을 확인하면 내가 설정한 경로가 아니다?</p>
<p><span class="highlight">이클립스 재실행</span>을 해서 다시 확인하면,</p>
{% endraw %}

![_18](https://user-images.githubusercontent.com/34805973/39973962-26c9cada-5760-11e8-8e50-c8220f8d9d8c.PNG)

{% raw %}
<p>내가 설정한 경로로 잡혀 있는 것을 확인 할 수 있다.</p>
<h4>Maven target 폴더 제외</h4>
<p>svn 사용 시 target 이라는 폴더까지 같이 커밋되지 않기 위해 하는 설정으로, Maven 사용하여 프로젝트 진행하면 target이라는 폴더가 생기는데 프로젝트 컴파일한 파일이 저장된다고 한다. 그런데 프로젝트 형상관리 할 때 컴파일된 결과까지 커밋할 필요 없고 개발소스만 관리되면 되므로 target 폴더를 제외하고자 하는 것.</p>
{% endraw %}

![_19](https://user-images.githubusercontent.com/34805973/39973963-26f4cd8e-5760-11e8-905d-a146c8b87d00.PNG)

{% raw %}
<p>Windows → Preferences → team 검색 → Add Pattern → <span class="highlight">*/target/*</span> 추가</p>
{% endraw %}

![_20](https://user-images.githubusercontent.com/34805973/39973964-2723125c-5760-11e8-99b8-159e775bdb04.PNG)

{% raw %}
<p>체크 후 OK</p>
{% endraw %}

