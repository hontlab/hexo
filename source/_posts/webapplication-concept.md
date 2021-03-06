---
title: 웹어플리케이션 개념 및 구성요소
date: 2018-03-29 15:56:20
categories: jsp
tags: [웹어플리케이션, 웹, 인터넷, CGI]
description: 웹어플리케이션이란 HTML(정적인 언어)의 한계를 벗어나 다양한 동적인 응답을 생성하고 처리할 수 있는 프로그램입니다.
---
{% raw %}

<h2>웹</h2>
<p>거미줄처럼 연결된 망을 통해 사용자(구성요소[요청자(클라이언트)/제공자(서버)])끼리 정보를 공유하기 위한 <span class="highlight">가상의 공간, 논리적인 의미의 공간</span>, sw, 한국</p>
<p>추가하여, 정보를 공유하기 위해선 공동(통용) 언어가 필요한데 클라이언트사이드 언어(HTML, 자바스크립트)와 동적으로 만드는 서버사이드언어(Java, SQL 등)가 존재</p>

<h3>사용자 구분</h3>
<h4>1) 클라이언트(브라우저, web agent)</h4>
<h5>역할</h5>
<ol>
	<li>사용자 대신하여 서버에 요청</li>
	<li>응답 데이터 받아와 해석</li>
</ol>
<h4>2) 서버</h4>
<h5>역할</h5>
<ol>
	<li>(클라이언트 요청 대기)리스닝</li>
	<li>요청자원 찾기</li>
	<li>자원을 0,1로 바꾸어 응답, 내보낼 수 있는 프로토콜로 포장</li>
	<li>톰캣을 통해 서블릿 객체 만들어 doxxx메서드 호출</li>
</ol>

<h5>구분</h5>
<ul>
	<li>웹 서버 - 정적 요청 처리, Apache</li>
	<li>웹 어플리케이션 서버(WAS) - 동적 요청 처리, Tomcat</li>
</ul>

<h2>인터넷(inter+net)</h2>
<p>전세계를 하나의 거미줄로 연결한 망, <span class="highlight">물리적인 의미의 공간</span>, hw, 한반도, 인터넷이 없다면 웹도 없음</p>

<h2>웹어플리케이션</h2>
<p>HTML(정적인 언어)의 한계를 벗어나 다양한 동적인 응답을 생성하고 처리할 수 있는 프로그램</p>
<p>구성요소로는 웹서버, 웹어플리케이션서버, 데이터베이스, 웹브라우저</p>

<h3>CGI방식과 어플리케이션 서버 방식(동작구조에 따른 구분)</h3>
<h4>1) CGI방식(정적방식에서 동적방식으로의 첫번째 방식)</h4>
<ul>
	<li>CGI(Common Gateway Interface) : 웹서버와 프로그램 사이에 정보를 주고받는 규칙</li>
	<li>웹서버가 직접 프로그램을 호출하는 구조</li>
	<li>요청이 늘어날 때마다 동시에 호출되는 프로그램 수가 증가(<span class="highlight">멀티프로세싱 방식</span>), 동시 처리 개수가 제한되는 단점</li>
</ul>

<h4>2) 어플리케이션 방식(확장 CGI방식, 대표방식이 자바기반 서블릿)</h4>
<ul>
	<li>웹서버가 직접 프로그램을 호출하지 않고, 어플리케이션 서버를 통해 간접적으로 실행하는 구조</li>
	<li><span class="highlight">멀티쓰레딩 방식</span>(여러 요청이 동시에 발생하더라도 이를 처리할 프로그램이 하나만 메모리에 로딩되므로 전체적인 부하가 줄어 CGI방식에 비해 동시 처리 가능한 전체 처리량 증가, 대량 트래픽 처리해야하는 시스템에 적합)</li>
	<li>웹서버는 클라이언트의 요청을 어플리케이션 서버에 전달</li>
	<li>어플리케이션서버는 웹어플리케이션을 실행 후 그 결과를 다시 웹서버에 전달</li>
	<li>웹서버는 클라이언트로 응답을 재전송하는 방식으로 동작</li>
</ul>

<h3>실행코드 방식과 스크립트 방식(구현 및 실행방식에 따른 구분)</h3>
<h4>1) 실행코드 방식</h4>
<ul>
	<li>컴파일된 실행 프로그램</li>
	<li>컴파일된 기계어 코드 직접 실행</li>
	<li>소스코드를 다시 컴파일 해야함</li>
	<li>C기반 CGI 프로그램</li>
	<li>일반적으로 CGI방식</li>
</ul>

<h4>2) 스크립트 방식</h4>
<ul>
	<li>컴파일 되지 않은 스크립트 코드</li>
	<li>스크립트 코드를 번역한 뒤 실행, 최초 요청 시 한번 실행</li>
	<li>스크립트 코드만 고치면 됨</li>
	<li>JSP, APS.net, PHP, Ruby 등</li>
	<li>어플리케이션 서버 방식</li>
</ul>

{% endraw %}


