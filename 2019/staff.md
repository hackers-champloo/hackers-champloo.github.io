---
home: 2019
layout: camp/layout
title: 実行委員会 ボランティアスタッフ
---

{% unless site.data.staffs2019 %}

# ボランティアスタッフを募集しています

 ハッカーズチャンプルーは、実行委員会の有志が手作りで作り上げるエンジニアのためのイベントです。是非一緒にイベントを盛り上げてください！

## 応募内容

 実行委員会には、以下のような仕事があります。イベントの数ヶ月前からイベント終了後まで様々な仕事があり、これを各自個人の空き時間で処理して行きます。

* イベント企画 / イベント全体の中の様々な企画を立案、実施していきます
* メディア対応 / Webサイト運営から写真撮影・ソーシャルメディアなどの対外的情報発信をサポート
* 開発合宿支援 / 合宿会場や参加者の取りまとめやサポート
* カンファレンス支援 / カンファレンス会場の設営から受付・会場整理まで当日の運営をサポート
* 懇親会支援 / 会場整理や当日の運営をサポート

この他に、当日のみお手伝いをいただくボランティアスタッフもあります。

## ミーティングについて

ミーティングやタスク管理はほぼすべてオンラインで行われます。SlackやGoogle docsなどの取扱に慣れている必要があります。

## お申込み

当日ボランティアスタッフは6/29のカンファレンスおよび懇親会の準備や運営をお手伝い頂くスタッフです。

*  主なタスクは、受付業務、進行業務、会場設営・撤収などです。
*  以下の特典があります。
   * スタッフ専用デザインのTシャツ
* 金銭的な報酬はありません。

[当日ボランティアスタッフのお申込みはこちら](https://docs.google.com/forms/d/e/1FAIpQLSeExTG2U-nGKpyAj_4dt0ueHUHz8J6k-6X7VFZVs92_js30KQ/viewform)


{% else %}

# ハッカーズチャンプルーはボランティアに支えられ運営されています

## ハッカーズチャンプルー2019 実行委員会 コアメンバー

<ul class="staffs">

{% for staff in site.data.staffs2019 %}
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


## ハッカーズチャンプルー2019 当日ボランティアスタッフ

<ul class="staffs">

{% for staff in site.data.staffs2019 %}
  {% if staff.kind == 'ボランティア' and staff.name %}
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


--------------------------------------------------------------------------------

ボランティアの皆様のご協力なしに、このイベントの運営は成り立ちません。

本当にありがとうございます。そしてスタッフ一同楽しんでください！

2019年6月18日 実行委員長 西島 幸一郎

{% endunless %}
