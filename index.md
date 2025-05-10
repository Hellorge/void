{% for file in site.static_files %}
    {% if file.path contains "works" %}
    <iframe class="demo-frame" src="{{ file.path | absolute_url }}"></iframe>
    <a href="{{ file.path | absolute_url }}">{{ file.basename }}</a>
    {% endif %}
{% endfor %}
