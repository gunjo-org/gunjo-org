---
layout: compress
---
<!DOCTYPE html>
<html lang="ja">
  {% include html-head.md %}
  <body>
    <div class="container">
      {% include header.md %}
      <main>
        {{ content }}
      </main>
      <small>&copy;&nbsp;{{ 'now' | date: "%Y" }}&nbsp;{{ site.title }}</small>
    </div>
  </body>
</html>
