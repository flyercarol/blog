---
layout: page
title: Blog Archive
---

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.date | date: "%B %Y" }} - {{ post.title }}</a></li>
      <li><a href="{{ post.url }}">{{ post.date | date: "%B %Y" }} - {{ post.title }, check here}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

Test here:
baseurl
{{page.baseurl}}
<a href="{{ post.url }}">{post_url}</a>

<a href="{{ site.url }}">{site_url}</a>
relative
<a href="{{ page.url | relative_url }}">{relative_url}</a>
absollute
<a href="{{ page.url | absolute_url }}">{absolute_url}</a>

end here