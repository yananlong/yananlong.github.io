{% assign news_items = site.data.news %}
{% if include.count %}{% assign news_items = news_items | slice: 0, include.count %}{% endif %}
{% for item in news_items %}
- **{{ item.date }}:** {{ item.text }}
{% endfor %}
