---
home: 2025
layout: nocamp/layout
title: 実行委員会 ボランティアスタッフ
---

{% unless site.data.staffs2025 %}
{% else %}

# ハッカーズチャンプルーはボランティアに支えられ運営されています

## ハッカーズチャンプルー2025 実行委員会 コアメンバー

<ul class="staffs">

{% for staff in site.data.staffs2025 %}
  {% if staff.kind == 'コア' and staff.name %}
    {% if staff.link %}
      <li>
        <a href="{{ staff.link }}" target="_blank" rel="noopener">
          {% if staff.image %}<img src="{{ staff.image }}" alt="{{ staff.name }}"><br>{% endif %}
          {{ staff.name }}
        </a>
        {% if staff.text %}
          <p>{{ staff.text }}</p>
        {% endif %}
      </li>
    {% else %}
      <li>
        <span>{% if staff.image %}<img src="{{ staff.image }}" alt="{{ staff.name }}"><br>{% endif %}{{ staff.name }}</span>
        {% if staff.text %}
          <p>{{ staff.text }}</p>
        {% endif %}
      </li>
    {% endif %}
  {% endif %}
{% endfor %}

</ul>

{% assign staffs_on_the_day = site.data.staffs2025 | where:'kind','当日' %}
{% if staffs_on_the_day.last %}

## ハッカーズチャンプルー2025 当日ボランティアスタッフ

<ul class="staffs">

{% for staff in staffs_on_the_day %}
  {% if staff.name %}
    {% if staff.link %}
      <li>
        <a href="{{ staff.link }}" target="_blank" rel="noopener">
          {% if staff.image %}<img src="{{ staff.image }}" alt="{{ staff.name }}"><br>{% endif %}
          {{ staff.name }}
        </a>
        {% if staff.text %}
          <p>{{ staff.text }}</p>
        {% endif %}
      </li>
    {% else %}
      <li>
        <span>{% if staff.image %}<img src="{{ staff.image }}" alt="{{ staff.name }}"><br>{% endif %}{{ staff.name }}</span>
        {% if staff.text %}
          <p>{{ staff.text }}</p>
        {% endif %}
      </li>
    {% endif %}
  {% endif %}
{% endfor %}

</ul>
{% endif %}


--------------------------------------------------------------------------------

ボランティアのご協力なしに、このイベントは成立しません。

本当にありがとうございます。皆さんも一緒に楽しんでください！

2025年07月12日 実行委員長 西島 幸一郎

{% endunless %}
