---
layout: default
title: 参院選、東京選挙区
---

# 政治家の公約

{% for person in site.politicians %}
---

## {{ person.name }}

/assets/images/Okumura.jpg

**党:** {{ person.party }}

### 公約

{% for item in person.promises %}
- **{{ item.topic }}**: {{ item.description }}  

{% endfor %}

{% endfor %}





