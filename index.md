---
layout: default
title: tokyo politician 
---

# 政治家の公約

{% for person in site.politicians %}
---

## {{ person.name }}

![{{ person.name }}]({{ person.photo }}){: width="200" }

**党:** {{ person.party }}

### 公約

{% for item in person.promises %}
- **{{ item.topic }}**: {{ item.description }}  

{% endfor %}

{% endfor %}




