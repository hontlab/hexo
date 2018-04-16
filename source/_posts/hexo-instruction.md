---
title: hexo 명령어 정리
date: 2018-03-29 15:22:11
categories: hexo
tags: [hexo, 명령어]
description: hexo 명령어, 설치, 새포스트, 로컬서버, 생성, 배포 등 명령어가 있습니다.
---
{% raw %}

<h2>hexo설치</h2>
<pre>npm install -g hexo-cli</pre>

<h2>node.js 모듈 설치</h2>
<pre>npm install</pre>
<p>hexo 먼저 설치하고 진행해야, package.json을 참고하여 hexo에 필요한 모듈을 설치한다.</p>

<h2>새포스트 만들기</h2>
<pre>hexo new post (포스트명)</pre>

<h2>로컬서버 구동</h2>
<pre>hexo s</pre>

<h2>로컬서버 종료</h2>
<pre>ctrl+c 하고 y</pre>

<h2>원격저장소에 업로드 위한 파일 생성</h2>
<pre>hexo g</pre>

<h2>원격저장소에 업로드</h2>
<pre>hexo d</pre>
<p>만약 fatal:HttpRequestException encountered. 오류 발생할 경우, 윈도우 보안 관련 이슈로 윈도우에서 공식적으로 제공하는 <a href="https://github.com/Microsoft/Git-Credential-Manager-for-Windows/releases/tag/v1.14.0" target="_blank">Git Credential Manager For Windows v.1.14.0(GCMW-1.14.0.exe)</a> 다운받아 설치하면 해결 가능</p>

{% endraw %}


