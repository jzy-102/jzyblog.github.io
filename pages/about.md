---
layout: page
title: About
description: 个人博客
keywords: Jzy, 江子怡
comments: true
menu: 关于
permalink: /about/
---

开源课程设计

仰慕「优雅编码的艺术」。

坚信熟能生巧，努力改变人生。

## 联系
GitHub:jzy-102
email:3091987996@qq.com
tel:18110785273

疑难解答
<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
{% if site.url contains 'mazhuang.org' %}
<li>
微信公众号：<br />
<img style="height:192px;width:192px;border:1px solid lightgrey;" src="{{ site.url }}/assets/images/qrcode.jpg" alt="闷骚的程序员" />
</li>
{% endif %}
</ul>


## Skill Keywords

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
