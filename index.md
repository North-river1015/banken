---
layout: default
title: 参院選、東京選挙区
---

# 参議院選挙　東京選挙区

{% for person in site.politicians %}
---

## {{ person.name }}

/assets/images/Okumura.jpg

{{ person.party }}

### 公約

{% for item in person.promises %}
- **{{ item.topic }}**: {{ item.description }}  

{% endfor %}

{% endfor %}





