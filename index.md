---
title: التعليمات المستضافة عبر الإنترنت
permalink: index.html
layout: home
---

# دليل المحتوى

تم سرد الارتباطات التشعبية لكل من التدريبات والعروض التوضيحية المعملية أدناه.

## الأنشطة المعملية

{% assign labs = site.pages | where_exp:"page", "page.url contains '/Instructions/Labs/Conversational-actions'" %}
| الوحدة النمطية | النشاط المعملي |
| --- | --- | 
{% للأنشطة في المعامل %}| {{ activity.lab.module }} | [{{ activity.lab.title }}{% if activity.lab.type %} - {{ activity.lab.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}

