---
title: iPhoneでUTokyo VPNを利用する 
---

このページでは，UTokyo VPNをiPhoneで利用する方法を説明します．

{% include_relative _subpage_beginning.md %}
## 準備編: UTokyo VPNの初期設定
{:#setup}

まずはUTokyo VPNに接続するために必要なアプリを端末にインストールし，初期設定を行います．手順は通常のiOSアプリと同様です．

**手順A:** [App Store](https://apps.apple.com/jp/app/cisco-anyconnect/id1135064690) にアクセスし，Cisco社のCisco AnyConnectというアプリをインストールします．

<img src="img/iphone01-app-store.png" alt="anyconnect in app store" style="margin:auto; border:solid 1px black;" />

**手順B:** インストールを終えてAnyConnectアプリを開くと，下の左図のような画面が出ることを確認します．これでインストールは完了です．なお，開く際に下の右図のように通知の送信について確認するウィンドウが表示されることがありますが，いずれを選択しても構いません．

<ul style="display: flex;">
<li style="list-style: none;">
  <img src="img/iphone02-setup_home.png" alt="anyconnect home finished setting" style="margin:auto; width:95%; border:solid 1px black;" /></li>
<li style="list-style: none;">
  <img src="img/iphone03-setup_home_popup_notify.png" alt="anyconnect notification" style="margin:auto; width:95%; border:solid 1px black;" /></li>
</ul>

**手順C:** アプリを起動した直後の画面で左上の「接続」をタップし，続いて表示される画面で「VPN接続の追加」をタップすると，下図のようなウィンドウが表示されます．「サーバ」の横の入力欄をタップして **vpn1.adm.u-tokyo.ac.jp** と入力します．

<img src="img/iphone04-setup_home_connections_add-vpn-connection.png" alt="anyconnect vpn setting window" style="margin:auto; border:solid 1px black;" />

**手順D:** 「保存」を押すと，下図のようにVPN構成の追加を求められるので，内容の確認の上で「許可」を押します．さらに追加でTouch IDによる認証などを求められることもありますので，その際は認証を行ってください．

<img src="img/iphone05-setup_home_connections_add-vpn-connection_popup_config.png" alt="anyconnect authentication window" style="margin:auto; border:solid 1px black;" />


## 利用編: UTokyo VPNへの接続
{:#connect}

以下の手順はVPNを利用するたびに必要です．特に端末を起動した直後に自動的にVPNに接続されるわけではありませんので，ご注意ください．

**手順E:** 下記左図のように画面上部の「接続」に「vpn1.adm.u-tokyo.ac.jp」と記載されていることを確認してください．次に「AnyConnect VPN」の横のトグルボタンをONにして，下記右図のようにUTokyo Accountの認証ウィンドウが表示されたら，ご自身のUTokyo Accountでサインインしてください．前回のアクセスから時間をおかずに起動した場合は，この画面が表示されないで直ちにVPN接続が開始されることもあります．

<ul style="display: flex;">
<li style="list-style: none;">
  <img src="img/iphone06-home_disconnected.png" alt="anyconnect home finished setting" style="margin:auto; width:95%; border:solid 1px black;" /></li>
<li style="list-style: none;">
  <img src="img/iphone07-signin_.png" alt="anyconnect authentication window" style="margin:auto; width:95%; border:solid 1px black;" /></li>
</ul>

{% include_relative _help_mfa.html %}
{% include_relative _help_multiple_users.html %}

**手順F:** 認証に成功すれば，VPNへの接続は完了です．ZoomやWebexなどVPNを経由する必要のない一部の通信や電子ジャーナルサイトなどを除く全ての通信は，このVPNを経由して，東京大学キャンパスネットワークに接続している状態で行われます．

**手順G:** 下記の画面のように「詳細」が「接続済み」と表示されていれば，お使いの端末はUTokyo VPNに接続している状態です．

<img src="img/iphone08-home_connected.png" alt="anyconnect finished connecting" style="margin:auto; border:solid 1px black;" />

VPNを切断する際は，この画面のトグルボタンをタップして「詳細」が「接続解除済み」になったことを確認してください．

---

[UTokyo VPN全体のページに戻る](.)
