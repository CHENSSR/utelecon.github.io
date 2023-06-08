---
title: Online Class / Web Conference Portal Site @ the University of Tokyo
top: true
sitemap: false
---

{% include layouts/header.html is_top = true %}

<main id="content">

  <h2>Getting Ready for ICT Systems</h2>
  <div class="cards">
    <a href="/en/oc/">For New Students</a>
    <a href="/en/faculty_members/">For Faculty Members</a>
    <a href="/en/improvement/">Improving Online Classes</a>
    <a href="/en/support/">Support Desk</a>
  </div>

  <h2>Pickup</h2>
  <div class="cards">
    <a href="/events/2022-09-14/">2022/09/14 Briefing Session: online conference and cloud tools <small>(only in Japanese)</small></a>
    <a href="/en/notice/2023/01-wifi">Changes in usage of UTokyo Wi-Fi due to renewal</a>
    <a href="/en/slack/">UTokyo Slack</a>
    <a href="/en/utokyo_vpn/">UTokyo VPN</a>
    <a href="/en/utokyo_account/mfa/">Using Multi-Factor Authentication for UTokyo Accounts</a>
  </div>

  <h3>Information on Beginning of Semester</h3>
  <div class="cards">
    <a href="/en/faculty_members/url">How to Announce Online Class URL (for Faculty Members)</a>
    <a href="/en/faculty_members/zoom_access_control">Restricting Access to Zoom Meeting Rooms for Online Classes <small>(for Faculty Members)</small></a>
    <a href="/en/oc/url">How to Obtain the Online Class URL (for Students)</a>
    <a href="/en/oc/join">How to join a online class <small>(for Students)</small></a>
  </div>

  <h2>Notice</h2>
  {% comment %} To add notice here, edit `_data/notice/en.yml` {% endcomment %}
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
    {%- endunless -%}
      <li>
        <span class="notice-date">{{ item.date }}</span>
        {{ item.content.en | default: item.content.ja | markdownify | replace: '<p>', '' | replace: '</p>', '' }}
      </li>
    {%- endfor %}
  </ul>

  <h2>ICT Systems</h2>
  <div class="top__systems">
    <ul>
      <li><a href="/en/utokyo_account/">UTokyo Account</a></li>
      <li><a href="/en/utas">UTAS</a></li>
      <li><a href="/en/itc_lms">ITC-LMS</a></li>
      <li><a href="/en/zoom/">Zoom</a></li>
      <li><a href="/en/webex/">Webex</a></li>
      <li><a href="/en/eccs_cloud_email">ECCS Cloud Email<small> (Google Workspace)</small></a></li>
      <li><a href="/en/microsoft/">UTokyo Microsoft License<small> (Microsoft 365)</small></a></li>
      <li><a href="/en/utokyo_wifi/">UTokyo Wi-Fi</a></li>
      <li><a href="https://www.ecc.u-tokyo.ac.jp/en/">ECCS Terminals</a></li>
    </ul>
  </div>
</main>

{% include layouts/footer.html %}