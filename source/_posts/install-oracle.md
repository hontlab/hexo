---
title: Oracle 설치
tags: [오라클, Oracle, 설치]
date: 2018-05-14 11:52:56
categories: setting
description: Oracle 설치
---
![_1](https://user-images.githubusercontent.com/34805973/39978331-d40f9188-577a-11e8-9af0-6c363d61e681.PNG)

{% raw %}
<p>오라클 사이트(<a href="https://www.oracle.com/index.html" target="_blank">https://www.oracle.com/index.html</a>) 접속하여 파일 다운로드 진행</p>
<p>여기서는 <span class="highlight">Database 11g Enterprise/Standard Editions</span>을 받는다. 아래 쭉 내려보면 차례차례 이동하여 해당 파일을 바로 받을 수 있는 링크를 걸어놨습니다.</p>
{% endraw %}

![_2](https://user-images.githubusercontent.com/34805973/39978332-d4345162-577a-11e8-848b-ed452383e5db.PNG)

![_3](https://user-images.githubusercontent.com/34805973/39978333-d45ca4f0-577a-11e8-9e38-ed4af79e4037.PNG)

![_4](https://user-images.githubusercontent.com/34805973/39978334-d48223b0-577a-11e8-8d75-4c8a821954d4.PNG)

![_5](https://user-images.githubusercontent.com/34805973/39978335-d4a85bca-577a-11e8-91c2-b3025d8a181e.PNG)

{% raw %}
<p>여기까지의 링크(<a href="http://www.oracle.com/technetwork/database/enterprise-edition/downloads/index.html" target="_blank">http://www.oracle.com/technetwork/database/enterprise-edition/downloads/index.html</a>)</p>

<p>찾아보니 '클라이언트(client)' 버전을 설치해서 DB에 접속 할 수 있지만, <span class="highlight">'데이터베이스(server)' 버전을 설치하면 컴퓨터에서 자신의 DB를 운영/관리할 수 있게 됩니다.</span></p>

<p>클라이언트는</p>
<ul>
	<li>서버 이외의 컴퓨터에서 서버 즉 데이터베이스에 접근하기 위한 프로그램.</li>
	<li>오라클 서버로 접속하기 위한 매개체로 보면 됩니다.</li>
	<li>다른 서버에서 오라클 클라이언트를 설치하고 오라클 서버의 정보를 입력하면 오라클 서버로 접속이 가능하게 됩니다.</li>
	<li>즉, 오라클 서버가 있고 오라클 클라이언트로 연계하여 사용하는 것.</li>
</ul>
 <p><span class="highlight">데이터베이스 버전을 설치하면 클라이언트는 추가로 설치할 필요는 없습니다.</span> (데이터베이스 버전에 클라이언트가 포함되어 있다고 생각하면 됩니다. 데이터베이스는 설치파일이 약 2GB이며, 클라이언트는 설치파일이 약 1.2GB입니다.)</p>

{% endraw %}

![_6](https://user-images.githubusercontent.com/34805973/39978337-d4cf9b7c-577a-11e8-81a5-e1c4ae8579b3.PNG)

{% raw %}
<p>다운 받으려면, 오라클 로그인을 해야 합니다.</p>
{% endraw %}

![_7](https://user-images.githubusercontent.com/34805973/39978338-d4f4e620-577a-11e8-87e6-db6255798fd1.PNG)

![_8](https://user-images.githubusercontent.com/34805973/39978288-c0feeee0-577a-11e8-870a-76a8f971fb80.PNG)

![_9](https://user-images.githubusercontent.com/34805973/39978289-c125dffa-577a-11e8-98c2-5c6739edeba9.PNG)


{% raw %}
<p>두 개의 zip파일 압축을 풀면, database라는 하나의 폴더에 함께 압축이 풀립니다. 이전에는 서로 다른 곳에 풀려서 한 폴더로 옮겨줘야 했다는데 지금은 개선된 것 같습니다.</p>
{% endraw %}

![_10](https://user-images.githubusercontent.com/34805973/39978290-c150fc76-577a-11e8-9a82-42f256354536.PNG)

{% raw %}
<p>database 폴더 내 setup.exe 파일 실행</p>
{% endraw %}

![_11](https://user-images.githubusercontent.com/34805973/39978291-c1760264-577a-11e8-9f51-a69ac100d5d4.PNG)

![_12](https://user-images.githubusercontent.com/34805973/39978292-c19f57a4-577a-11e8-967b-035dc9952ba6.PNG)

![_13](https://user-images.githubusercontent.com/34805973/39978293-c1c5b02a-577a-11e8-9d25-6eb9371dac9c.PNG)

![_14](https://user-images.githubusercontent.com/34805973/39978294-c1ee43d2-577a-11e8-8621-1bdd9a4a2f2d.PNG)

![_15](https://user-images.githubusercontent.com/34805973/39978295-c2164c2e-577a-11e8-8db3-01ee3a5ab648.PNG)

![_16](https://user-images.githubusercontent.com/34805973/39978296-c23cee1a-577a-11e8-8f2f-85fd3e08f1f4.PNG)

![_17](https://user-images.githubusercontent.com/34805973/39978297-c2644a46-577a-11e8-9139-a8c696999900.PNG)


{% raw %}
<p>관리자 계정명과 비밀번호 입력</p>
<p>여기선, root로 했는데 보통 sys로 많이 하는 것 같습니다.</p>
{% endraw %}

![_18](https://user-images.githubusercontent.com/34805973/39978298-c28abb9a-577a-11e8-93ff-f06b83f3e3b7.PNG)

![_19](https://user-images.githubusercontent.com/34805973/39978299-c2b1a46c-577a-11e8-964f-6e313dff8761.PNG)

![_20](https://user-images.githubusercontent.com/34805973/39978300-c2da0c54-577a-11e8-8b8d-6aeaa8cc5587.PNG)

![_21](https://user-images.githubusercontent.com/34805973/39978301-c302108c-577a-11e8-9ae1-84d39bbe523a.PNG)

![_22](https://user-images.githubusercontent.com/34805973/39978302-c32a3f4e-577a-11e8-9fc8-9ae1c01c75c5.PNG)


{% raw %}
<p>오라클 연결 테스트를 위해 사용할 계정(SCOTT) 잠금해제를 위해 비밀번호 관리 버튼 클릭(테스트를 위한 것이라 필수사항은 아님)</p>
{% endraw %}

![_23](https://user-images.githubusercontent.com/34805973/39978303-c34fde2a-577a-11e8-8393-8767e30cc2eb.PNG)

{% raw %}
<p>SCOTT 계정 체크 해제</p>
{% endraw %}

![_24](https://user-images.githubusercontent.com/34805973/39978304-c37604c4-577a-11e8-8600-c89f5f82f409.PNG)

![_25](https://user-images.githubusercontent.com/34805973/39978305-c39b425c-577a-11e8-886d-b2c8ca94b451.PNG)

{% raw %}
<p>sqlplus 실행 후, 관리자로 로그인 명령어(<span class="highlight">sqlplus "/as sysdba"</span>) 수행</p>
{% endraw %}

![_26](https://user-images.githubusercontent.com/34805973/39978306-c3c0e052-577a-11e8-968f-679dcad25f05.PNG)

{% raw %}
<p>사용자 계정 로그인 명령어(<span class="highlight">conn scott/tiger</span>) 수행(conn 계정명/비밀번호)</p>
<p>비밀번호가 만료됐다고 비밀번호 바꾸라 하니 바꿉니다.</p>
{% endraw %}

![_27](https://user-images.githubusercontent.com/34805973/39978307-c3e6daaa-577a-11e8-83d6-6e9ed4c19772.PNG)

{% raw %}
<p>scott 데이터 조회를 위한 명령어(<span class="highlight">select * from dept;</span>) 수행</p>
<p>다음과 같이 부서 데이터가 조회되는 것을 확인할 수 있습니다.</p>
{% endraw %}

![_28](https://user-images.githubusercontent.com/34805973/39978308-c40e148a-577a-11e8-9033-d2d6c44619dc.PNG)

{% raw %}
<p>종료할 때는 exit를 2번 입력하면 종료</p>
<p>다음에는 항상 sqlplus 명령창을 통해 DB사용하기 불편하니, DBMS(DataBase Management System)로 많이 쓰이는 Oracle SQL Developer 설치 방법을 포스팅 하고자 합니다.</p>
{% endraw %}