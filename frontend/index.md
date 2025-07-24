---
layout: default
title: All Politicians
---

# Politicians and Manifestos

{% for person in site.politicians %}
---

## {{ person.name }}

![{{ person.name }}]({{ person.photo }}){: width="200" }

**Party:** {{ person.party }}

### Manifesto

{% for item in person.promises %}
- **{{ item.topic }}**: {{ item.description }}  
  {% if item.status == "completed" %} ✅ Completed  
  {% elsif item.status == "not_accomplished" %} ❌ Not Accomplished  
  {% else %} ⚪ Unassessed  
  {% endif %}
{% endfor %}

{% endfor %}
