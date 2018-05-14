---
title: Spring 설치(이클립스 플러그인 ver)
tags: [Spring, 설치]
date: 2018-05-14 10:59:52
categories: setting
description: Spring 설치
---
{% raw %}
<p>Spring을 설치하는 방법으로는,</p>
<ul>
	<li>Spring 사이트에서 제공하는 STS(Spring Tool Suite)을 다운</li>
	<li class="highlight">이클립스에서 플러그인으로 다운</li>
</ul>
<p>여기서는 이클립스 마켓을 통해 Spring 플러그인을 다운받아 사용하는 것으로 하겠다.</p>
{% endraw %}

![_1](https://user-images.githubusercontent.com/34805973/39974831-29266d50-5766-11e8-9adc-02c3f36a7221.png)

{% raw %}
<p>Help → Eclipse Marketplace</p>
{% endraw %}

![_2](https://user-images.githubusercontent.com/34805973/39974832-294d569a-5766-11e8-8447-da897471e98b.png)

{% raw %}
<p>sts 검색 후 install</p>
{% endraw %}

![_3](https://user-images.githubusercontent.com/34805973/39974833-2972874e-5766-11e8-9aba-3e8f210bffe9.png)

![_4](https://user-images.githubusercontent.com/34805973/39974834-2998e1dc-5766-11e8-8d4e-0a37b618e7ce.png)

![_5](https://user-images.githubusercontent.com/34805973/39974835-29bfaf06-5766-11e8-9fc3-0ae6e74fcffc.png)

![_6](https://user-images.githubusercontent.com/34805973/39974836-29e68392-5766-11e8-90f1-c269701ac341.png)

![_7](https://user-images.githubusercontent.com/34805973/39974837-2a0b951a-5766-11e8-8f27-7b9842033c39.png)

{% raw %}
<p>이클립스 재실행</p>
<p>이제 Spring이 잘 설치됐는 지 확인해보고자 아래처럼 수행</p>
{% endraw %}

![_8](https://user-images.githubusercontent.com/34805973/39974838-2a30ace2-5766-11e8-8bd4-94a5c3982296.png)

{% raw %}
<p>File → New → Other</p>
{% endraw %}

![_9](https://user-images.githubusercontent.com/34805973/39974839-2a5abda2-5766-11e8-91b0-e52fa553853b.png)

{% raw %}
<p>spring 검색</p>
{% endraw %}

![_1](https://user-images.githubusercontent.com/34805973/39974846-36f37054-5766-11e8-80f8-d921f0f86c0c.PNG)

{% raw %}
<p><span class="highlight">Spring Legacy Project</span> 선택</p>
<p>그냥 Legacy 뜻이 뭔지 궁금해서 찾아보니,</p>
{% endraw %}
![_2_2](https://user-images.githubusercontent.com/34805973/39975305-ba7ee118-5768-11e8-8665-d7f663958d3d.PNG)

{% raw %}
<p>Spring으로 프로젝트 기본 세팅이 되니 Legacy로 이름 지었나 보다.</p>
{% endraw %}

![_2](https://user-images.githubusercontent.com/34805973/39974847-3719ce34-5766-11e8-9c4a-53ee8329ae23.PNG)

{% raw %}
<p>프로젝트명 입력하고, <span class="highlight">Spring MVC Project</span> 선택</p>
{% endraw %}

![_3](https://user-images.githubusercontent.com/34805973/39974848-373f334a-5766-11e8-990e-ff4d9bea8317.PNG)

![_4](https://user-images.githubusercontent.com/34805973/39974849-37672896-5766-11e8-9994-7c9bd90e714e.PNG)

{% raw %}
<p>패키지명 입력</p>
{% endraw %}

![_5](https://user-images.githubusercontent.com/34805973/39974850-378f7bde-5766-11e8-8ffe-305b7dfe166a.PNG)

{% raw %}
<p>우측하단 빌드가 끝나면,</p>
{% endraw %}

![_6](https://user-images.githubusercontent.com/34805973/39974851-37b83312-5766-11e8-92ba-024e45f1c9b4.PNG)

{% raw %}
<p>톰캣 서버에 프로젝트 추가</p>
{% endraw %}

![_7](https://user-images.githubusercontent.com/34805973/39974852-37e0cb1a-5766-11e8-8114-49953f982be0.PNG)

![_8](https://user-images.githubusercontent.com/34805973/39974853-3808e9a6-5766-11e8-8421-a90fed74f03a.PNG)

![_9](https://user-images.githubusercontent.com/34805973/39974854-3831d564-5766-11e8-9e18-bf42dfaafffe.PNG)

{% raw %}
<p>톰캣 서버 구동</p>
{% endraw %}

![_10](https://user-images.githubusercontent.com/34805973/39974855-385bcdce-5766-11e8-9ab4-13b5bf7022f0.PNG)

![_11](https://user-images.githubusercontent.com/34805973/39974857-38958cda-5766-11e8-97c6-0ddcc3051ec7.PNG)

{% raw %}
<p>the required server component failed to start so tomcat is unable to start<br>org.apache.catalina.lifecycleexception: failed to start component [standardserver[8005]]</p>
<p>아무 오류 없이 나왔다면 다행이지만, 다음과 같이 오류가 났다면 해결법은.. 내가 검색하면서 사용했던 방법을 나열해 본다.</p>
<ul>
	<li>프로젝트와 서버 clean // (필자의 경우) 미해결</li>
	<li>서버 포트번호 변경 // (필자의 경우) 미해결</li>
	<li>서버 지우고, 프로젝트 지우고, 메이븐 로컬저장소 폴더내 파일 다 지우고 <span class="highlight">프로젝트, 서버 새로 세팅 // 해결</span></li>
</ul>
{% endraw %}

![_12](https://user-images.githubusercontent.com/34805973/39974859-38bb398a-5766-11e8-8d26-3f54777ac76f.PNG)

