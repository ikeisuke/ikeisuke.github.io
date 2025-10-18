layout: page
title: Home
---

# アプリのドキュメントとポリシー

以下のアプリのポリシーやドキュメントを公開しています。

## アプリ一覧

<ul>
{% for app in site.data.apps %}
  <li>
    <strong>{{ app.name }}</strong>
    {% if app.links.privacy %}
      — <a href="{{ app.links.privacy }}">プライバシーポリシー</a>
    {% endif %}
  </li>
{% endfor %}
</ul>
