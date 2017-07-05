---
layout: page
title: Posts
permalink: /posts/
---
<table>
<tbody>
{% for post in site.posts limit:5 %}  
<tr>
<td>
<a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
</td>
<td>
{{ post.date | date: "%m/%d/%Y" }}
</td>
</tr>
{% endfor %}  
</tbody>
</table>
