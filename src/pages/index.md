---
title: オンライン授業・Web会議 ポータルサイト @ 東京大学
sitemap: false
description: 本サイトは，東京大学におけるオンライン授業やWeb会議に関する情報をワンストップで得られることを目指すサイトです．
top: true
---

<h2>まずはここから</h2>
  <div class="cards">
    <a href="/oc/">大学生活に必要な情報システムの準備について<small>（新入生向け）</small></a>
    <a href="/faculty_members/">東京大学における情報システムの準備について<small>（教員向け）</small></a>
    <a href="/online/">オンラインを活用するために</a>
    <a href="/support/">サポート窓口</a>
  </div>

  <h2>ピックアップ</h2>
  <div class="cards">
    <a href="/events/2023-03-15/">オンラインでも対面でも活用！Web会議・クラウドツールの説明会 <small>(2023/03/15)</small></a>
    <a href="/notice/2023/01-wifi">UTokyo Wi-Fiの更新に伴う利用方法変更のお知らせ</a>
    <a href="/utokyo_account/mfa">UTokyo Accountにおける多要素認証の利用について</a>
    <a href="/slack/">UTokyo Slack</a>
    <a href="/utokyo_vpn/">UTokyo VPN</a>
    <a href="/online/topics/generative-ai">生成系AI（ChatGPT等）関連情報</a>
  </div>

  <h3>授業にあたって</h3>
  <div class="cards">
    <a href="/faculty_members/url">授業URLの連絡方法（教員向け）</a>
    <a href="/faculty_members/zoom_access_control">授業におけるZoom会議室の入室制限<small>（教員向け）</small></a>
    <a href="/zoom/license">Zoomの追加ライセンス<small>（301人以上のミーティング・ウェビナー）</small></a>
    <a href="/oc/url">授業URLの連絡方法（学生向け）</a>
    <a href="/oc/join">オンライン授業への入室方法<small>（学生向け）</small></a>
    <a href="/oc/rooms">オンライン授業の受講に利用可能な教室の一覧</a>
  </div>

  <h3>新着記事</h3>
  <!--
    概ね次の基準で掲載する
    - /articles/ 以下のページのみを「記事」と考え掲載対象とする
    - 新しい記事から古い記事の順に掲載する
    - 同時に公開された記事は同時に掲載開始し同時に掲載終了する
    - 常に2記事以上を掲載する
    - 目安としては3記事から6記事程度を掲載する
  -->
  <div class="cards">
    <a href="/articles/copyright/">学校・その他教育機関における著作権の取り扱い</a>
    <a href="/articles/itc-lms/">学習管理システムの概要を知る，ITC-LMSを活用する</a>
    <a href="/articles/group-discussion/">オンラインのグループディスカッションで生じやすい問題とその対策案</a>
    <a href="/articles/group-discussion-worksheet/">オンラインのグループディスカッションでワークシートを活用する</a>
    <a href="/articles/gas/">GAS（Google Apps Script）を使ってみましょう</a>
    <a href="/articles/gas/copy">GASを使ってGoogleドライブでファイルとフォルダを複製する方法</a>
  </div>

  <h3>オンライン授業の実践など</h3>
  <div class="cards">
    <a href="/good-practice/">グッドプラクティス</a>
    <a href="/events/luncheon/">オンライン授業情報交換会</a>
    <a href="/questionnaire/">オンライン授業に関するアンケート</a>
  </div>

  <h2>お知らせ</h2>
  {% comment %} お知らせの追加は `_data/notice.yml` を編集してください {% endcomment %}
  <ul>
    {%- assign i = 0 -%}
    {%- assign j = 0 -%}
    {%- for item in site.data.notice -%}
      {%- if item.outdated -%}
        {%- continue -%}
      {%- endif -%}
    {%- assign i = i | plus: 1 -%}
    {%- unless i <= 4 or item.important -%}
      {%- continue -%}
    {%- endunless -%}
    {%- assign j=j | plus: 1 -%}
    {%- unless i <=16 and j <=8 -%}
      {%- break -%}
    {%- endunless %}
      <li>
        <span class="notice-date">{{ item.date }}</span>
        {{ item.content.ja | default: item.content.en | markdownify | replace: '<p>', '' | replace: '</p>', '' }}
      </li>
    {%- endfor %}
  </ul>
  <a href="/notice/">過去のお知らせ一覧はこちら</a>

  <h2>東京大学のシステム</h2>
  <div class="top__systems">
    <ul>
      <li><a href="/utokyo_account/">UTokyo Account</a>
      </li>
      <li><a href="/utas">UTAS</a></li>
      <li><a href="/itc_lms">ITC-LMS</a></li>
      <li><a href="/zoom/">Zoom</a></li>
      <li><a href="/webex/">Webex</a></li>
      <li><a href="/eccs_cloud_email">ECCSクラウドメール<small> (Google Workspace)</small></a></li>
      <li><a href="/microsoft/">UTokyo Microsoft License<small> (Microsoft 365)</small></a></li>
      <li><a href="/utokyo_wifi/">UTokyo WiFi</a></li>
      <li><a href="https://www.ecc.u-tokyo.ac.jp/">ECCS端末</a></li>
      <li><a href="/systems/#others">その他</a></li>
    </ul>
  </div>