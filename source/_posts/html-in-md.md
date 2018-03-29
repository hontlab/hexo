---
title: md(markdown)에 html태그 사용하는 방법
date: 2018-03-29 14:19:02
categories: hexo
tags: [hexo, md, html]
---
{% raw %}
<h2>문제상황</h2>
<p>md(markdown)는 html태그에 익숙치 않은 사람들에게는 마크업을 보다 쉽게 해주는 편리함이 있지만, html태그를 조금이라도 알거나 혹은 사용하려는 사람들에게는 <span class="highlight">md를 그대로 사용할 경우 html태그가 제대로 파싱되지 않는 불편함이 있습니다.</span> 예를 들어 뜻하지 않은 br태그가 들어간다든지 하는 경우입니다.</p>

<h2>해결방법</h2>
<p>hexo에서 제공하는 <a href="https://hexo.io/docs/tag-plugins.html" class="highlight">Tag Plugins</a>을 사용하면 됩니다. Tag Plugins 중에서 <span class="highlight">Raw</span>를 사용하면 되고 사용법은 아래와 같습니다.</p>
<p>If certain content is causing processing issues in your posts, wrap it with the raw tag to avoid rendering errors.</p>
<p class="highlight">결국 raw라는 태그로 감싸서 사용하면 html태그로 인식한다는 것입니다.</p>

{% endraw %}
	
	{% raw %}
html태그
{% endraw %}



	
	





