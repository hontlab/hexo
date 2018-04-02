---
title: git 명령어 정리
date: 2018-03-29 12:05:41
categories : git
tags: [git, 명령어]
description: git 명령어, 원격저장소 설정, 저장, 업로드, 다운로드 등 명령어가 있습니다.
---
{% raw %}

<h2>git 최초 사용을 위한 세팅</h2>
<pre>git init</pre>

<h2>원격저장소 정보 세팅</h2>
<pre>git remote add origin (원격저장소 url)</pre>

<h2>원격저장소에서 다운로드 할 경우</h2>
<h3>최초</h3>
<pre>git clone (원격저장소 url)</pre>
<h3>이후</h3>
<pre>git pull</pre>

<h2>git 설정 정보 확인</h2>
<pre>git config --list</pre>

<h2>git 업로드 전 수정 및 삭제 파일 감지</h2>
<pre>git status</pre>

<h2>로컬에서 수정파일 add</h2>
<pre>git add (수정파일명 or *[모든 파일])</pre>

<h2>로컬에서 수정파일 commit</h2>
<pre>git commit -m "메시지 내용"</pre>
<p class="highlight">커밋 전에 add하여야 커밋 가능</p>

<h2>git 업로드</h2>
<pre>git push -u origin master</pre>
<p class="highlight">svn의 commit과 달리 push까지 해줘야 실제 원격저장소에 업로드</p>

{% endraw %}