<head>
    <title>{% if page.title %}{{ page.title }} | {% endif %}{{ site.title }}{% if page.title %}{% else %} | {{ site.tagline }}{% endif %}</title>
    <meta name="description" content="{% if page.description %}{{ page.description }}{% elsif page.excerpt %}{{ page.excerpt | strip_html | strip_newlines | escape | normalize_whitespace | truncate: 160 }}{% else %}{{ site.description }}{% endif %}">
    <link rel="canonical" href="{{ site.url }}{{ page.url }}">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <meta name="color-scheme" content="light dark">
    <link rel="icon" href="/assets/icon.svg" type="image/svg+xml">
    <link rel="alternate" type="application/rss+xml" title="{{ site.title }}" href="/feed.xml">
    {% capture style %}
    {% include style.scss %}
    {% endcapture %}
    <style>
    {{ style | scssify }}
    </style>
</head>
