---
title: UTokyo VPN
---

## はじめに
{:#introduction}

UTokyo VPNは東京大学全学の教職員が利用できるVPNサービスです．学外で端
末からUTokyo VPNに接続すると，その端末は情報基盤センターに設置された
VPNゲートウェイを経由して通信を行うようになり，端末は仮想的に東京大学
キャンパスネットワークであるUTNETに接続されている状態になります．

UTokyo VPNを利用するには，まず自身の端末にVPNクライアントアプリケーショ
ンであるAnyConnectをインストールします．インストールしたアプリケーショ
ンを起動すると，UTokyo Accountの認証を経てVPNゲートウェイに接続し，端
末からの通信がVPN経由でUTNETを通じて外部と通信するようになります．

## 利用にあたって
{:#note}

**利用対象者:** UTokyo Accountを持つ東京大学 教職員

**情報セキュリティ教育:** [情報セキュリティ教
育](https://www.u-tokyo.ac.jp/adm/dics/ja/securityeducationvideo.html)
を受講しないと，UTokyo VPNを利用することはできません．毎年度実施される
情報セキュリティ教育を受講しなかった場合は`jouhousecurity.adm __at__
gs.mail.u-tokyo.ac.jp` (`__at__`は@に変更)へ連絡してください．

**多要素認証の有効化:** UTokyo VPNを利用するためには，UTokyo Accountの
多要素認証を有効にする必要があります．[Utokyo Accountにおける多要素認
証の利用につい
て](https://utelecon.adm.u-tokyo.ac.jp/utokyo_account/mfa/)を参照し，
UTokyo Accountの多要素認証を有効にしてください．

**利用できるコンピュータの種類:** UTokyo VPNに接続できるコンピュータは
WindowsおよびmacOSの下記のバージョンです．iPhoneやAndroidなどのスマー
トフォンでも利用可能ですが，現時点ではマニュアル等のサポートは提供して
おりません．
- Windows: Windows 8.1およびWindows 10 x86(32-bit) and x64 (64-bit)
- macOS: macOS 11.2 (or later), 10.15, and 10.14 (64-bit)


**電子ジャーナルへのアクセス:** UTokyo VPN経由で電子ジャーナル等にアク
セスすることはできません．附属図書館が契約・提供する電子ジャーナル・電
子ブック・データベースの学外からの利用については附属図書館ウェブサイト
[EZproxy（イージープロキシー）経由で利用する](https://www.lib.u-tokyo.ac.jp/ja/library/literacy/user-guide/campus/offcampus/ezproxy) を参照してください．


## Windows端末でUTokyo VPNを利用する
{:#utokyo-vpn-windows}

### 準備編: VPNクライアントアプリケーションのダウンロードとインストール
{:#utokyo-vpn-windows-setup}

まずはUTokyo VPNに接続するために必要なアプリケーションを端末にインストー
ルします．

**手順1:**
[https://vpn1.adm.u-tokyo.ac.jp](https://vpn1.adm.u-tokyo.ac.jp) にアク
セスします．すると下記のようにUTokyo Accountの認証ページが表示されるの
で，自身のUTokyo Accountでログインします．

<img src="img/win01-vpn1-login.png" alt="vpn1.adm login page"
	style="margin:auto; width:80%; border:solid 1px black;" />



**手順2:** ログインに成功すると，下記のようなAnyConnectのクライアント
アプリケーションをダウンロードするためのページが表示されるので，
Download for Windowsをクリックして，クライアントアプリケーションをダウ
ンロードしてください．

その後は他のWindows用アプリケーションと同様にインストールします．

<img src="img/win02-download-page.png" alt="anyconnect download page"
	style="margin:auto; width:80%; border:solid 1px black;" />

上記のダウンロードページが表示されず，真っ白なページが表示される場合は，
[こちらのページ](https://vpn1.adm.u-tokyo.ac.jp/+CSCOE+/logon.html?tgroup=utvpn-tunnel-group)にアクセスしてください



**手順3:** End User License Agreementでは，"I accept the terms in the
License Agreement"を選択し，Nextを押して次へ進んでください．

<ul style="display: flex;">
<li style="list-style: none;">
  <img src="img/win03-install-1.png" alt="anyconnect install window"
	style="margin:auto; width:95%; border:solid 1px black;" /></li>
<li style="list-style: none;">
  <img src="img/win04-install-2.png" alt="anyconnect install window"
	style="margin:auto; width:95%; border:solid 1px black;" /></li>
<li style="list-style: none;">
  <img src="img/win05-install-3.png" alt="anyconnect install window"
	style="margin:auto; width:95%; border:solid 1px black;" /></li>
</ul>


**手順4:** インストールが完了すると，アプリにVPNクライアントアプリケー
ションであるCisco AnyConnect Secure Mobility Clientが追加されています．

<img src="img/win06-cisco-on-task.png" alt="anyconnect as an installed app"
	style="margin:auto; width:75%; border:solid 1px black;" />

これで準備は完了です．


### 利用編: UTokyo VPNへの接続
{:#utokyo-vpn-windows-connect}

以下の手順はVPNを利用するたびに必要です. 特にPCを起動した直後に自動的
にVPNに接続されるわけではありませんので, ご注意ください.


**手順1:** 準備編でインストールしたCisco Anyconnect Secure Mobility
Clientを起動すると，下記のようなウィンドウが出てきます．VPN接続先とし
て **vpn1.adm.u-tokyo.ac.jp** と入力し，「Connect」ボタンをクリックし
ます．

<img src="img/win07-app-window-connect.png" alt="anyconnect window"
	style="margin:auto; width:75%; border:solid 1px black;" />

UTokyo VPN接続時は，そのままだとコンピュータの繋がっているローカルネッ
トワークへの通信もVPNを経由します．VPNに接続したままローカルネットワー
クに設置されたプリンタ等を利用したい場合は，まず上写真のウィンドウの左
下，歯車のボタンをクリックしてください．すると下記のようなウィンドウが
出てきます．このウィンドウの「Preferences」タブから，「Allow local
(LAN) access when using VPN (if configured)」にチェックをつけてくださ
い．

<img src="img/win08-anyconnect-win-pref.png" alt="anyconnect preference"
	style="margin:auto; width:75%; border:solid 1px black;" />

**手順2:** 「Connect」ボタンを押し，下記のようなUTokyo Accountの認証ウィ
ンドウが表示されたら自身のUTokyo Accountでログインしてください．

<img src="img/win09-anyconnect-login.png" alt="anyconnect authentication"
	style="margin:auto; width:75%; border:solid 1px black;" />


**手順3:** 手順2の後，下記のように「Connected: vpn1.adm.u-tokyo.ac.jp」
と表示するウィンドウが出てくると，VPNへの接続は完了です．ZoomやWebExな
どVPNを経由する必要のない一部の通信や電子ジャーナルサイトなどを除く全
ての通信は，このVPNを経由し，東京大学キャンパスネットワークに接続して
いる状態で行われます．

<img src="img/win10-vpn-connected.png" alt="anyconnect connected"
	style="margin:auto; width:75%; border:solid 1px black;" />



**手順4:** 再度Cisco AnyConnect Secure Mobility Clientをクリックし，現
在の状態を確認します．表示されたウィンドウで，下記のように「Connected
to vpn1.adm.u-tokyo.ac.jp」と表示されていれば，お使いの端末はUTokyo
VPNに接続している状態です．

VPNを切断する際は，このウィンドウの「Disconnect」ボタンをクリックして
ください．

<img src="img/win11-vpn-connected-window.png" alt="anyconnect connected window"
	style="margin:auto; width:75%; border:solid 1px black;" />



## macOS端末でUTokyo VPNを利用する
{:#utokyo-vpn-macos}

### 準備編: VPNクライアントアプリケーションのダウンロードとインストール
{:#utokyo-vpn-macos-setup}

まずはUTokyo VPNに接続するために必要なアプリケーションを端末にインストー
ルします．

**手順1:**
[https://vpn1.adm.u-tokyo.ac.jp](https://vpn1.adm.u-tokyo.ac.jp) にアク
セスします．すると下記のようにUTokyo Accountの認証ページが表示されるの
で，自身のUTokyo Accountでログインします．

<img src="img/mac01-vpn1-login.png" alt="vpn1.adm login page"
	style="margin:auto; width:80%; border:solid 1px black;" />


**手順2:** ログインに成功すると，下記のようなAnyConnectのクライアント
アプリケーションをダウンロードするためのページが表示されるので，
Download for macOSをクリックして，クライアントアプリケーションをダウ
ンロードしてください．

その後は他のmacOS用アプリケーションと同様にインストールします．

<img src="img/mac02-download-page.png" alt="anyconnect download page"
	style="margin:auto; width:80%; border:solid 1px black;" />

<img src="img/mac03-install-1.png" alt="anyconnect download page"
	style="margin:auto; width:80%; border:solid 1px black;" />

上記のダウンロードページが表示されず，真っ白なページが表示される場合は，
[こちらのページ](https://vpn1.adm.u-tokyo.ac.jp/+CSCOE+/logon.html?tgroup=utvpn-tunnel-group)にアクセスしてください



**手順3:** AnyConnectのインストールの途中で，下記のような「ブロックさ
れたAnyConnectシステム拡張」というウィンドウがでる場合があります．その
際は表示される手順にしたがって，「システム設定」→「セキュリティとプラ
イバシー」のペインに表示されているCisco AnyConnect Socket Filterに関す
る許可を行なってください． また右のようなウィンドウが表示されますので，
これも許可をしてください．

<ul style="display: flex;">
<li style="list-style: none;">
  <img src="img/mac04-install-2.png" alt="blocking anyconnect"
	style="margin:auto; width:95%; border:solid 1px black;" /></li>
<li style="list-style: none;">
  <img src="img/mac05-install-3.png" alt="warning for anyconnect socket filter"
	style="margin:auto; width:95%; border:solid 1px black;" /></li>
</ul>


**手順4:** インストールが完了すると，アプリケーションフォルダに「Cisco」
というフォルダが作成され，その中にAnyConnectのクライアントアプリケーショ
ンであるCisco AnyConnect Secure Mobility Client.appがインストールされ
ています．

<img src="img/mac06-cisco-on-app.png" alt="anyconnect as an installed app"
	style="margin:auto; border:solid 1px black;" />

これで準備は完了です．

macOS 11 Big Sur以降のmacOS端末にAnyConnectのクライアントアプリケーショ
ンをインストールすると，「システム環境設定」→「ネットワーク」に下記の
ような Cisco AnyConnect Socket Filter という3つの拡張機能が追加されま
す．これらの拡張機能はUTokyo VPN接続時に通信を振り分けるために必要な機
能として常駐しており，通信内容の記録やホスト外への情報送付も行いません．
またこれらはUTokyo VPNに接続しているか否かに関わらず常時接続状態になり
ます．

<img src="img/mac07-macos-pref.png" alt="running anyconnect socket filter"
	style="margin:auto; width:75%; border:solid 1px black;" />


### 利用編: UTokyo VPNへの接続
{:#utokyo-vpn-macos-connect}

以下の手順はVPNを利用するたびに必要です. 特にPCを起動した直後に自動的
にVPNに接続されるわけではありませんので, ご注意ください.


**手順1:** 準備編でインストールしたCisco Anyconnect Secure Mobility
Clientを起動すると，下記のようなウィンドウが出てきます．VPN接続先とし
て **vpn1.adm.u-tokyo.ac.jp** と入力し，「Connect」ボタンをクリックし
ます．

<img src="img/mac08-app-window-connect.png" alt="anyconnect window"
	style="margin:auto; width:75%; border:solid 1px black;" />

UTokyo VPN接続時は，そのままだとコンピュータの繋がっているローカルネッ
トワークへの通信もVPNを経由します．VPNに接続したままローカルネットワー
クに設置されたプリンタ等を利用したい場合は，まず上写真のウィンドウの左
下，歯車のボタンをクリックしてください．すると下記のようなウィンドウが
出てきますので，「Allow local (LAN) access when using VPN (if
configured)」にチェックをつけてください．

<img src="img/mac09-anyconnect-mac-pref.png" alt="anyconnect preference"
	style="margin:auto; width:60%; border:solid 1px black;" />

**手順2:** 「Connect」ボタンを押し，下記のようなUTokyo Accountの認証ウィ
ンドウが表示されたら自身のUTokyo Accountでログインしてください．

<img src="img/mac10-anyconnect-login.png" alt="anyconnect authentication"
	style="margin:auto; width:75%; border:solid 1px black;" />


**手順3:** 認証に成功すれば，VPNへの接続は完了です．ZoomやWebExなどVPN
を経由する必要のない一部の通信や電子ジャーナルサイトなどを除く全ての通
信は，このVPNを経由して，東京大学キャンパスネットワークに接続している
状態で行われます．


**手順4:** 再度Cisco AnyConnect Secure Mobility Clientをクリックし，現
在の状態を確認します．表示されたウィンドウで，下記のように「Connected
to vpn1.adm.u-tokyo.ac.jp」と表示されていれば，お使いの端末はUTokyo
VPNに接続している状態です．

VPNを切断する際は，このウィンドウの「Disconnect」ボタンをクリックして
ください．

<img src="img/mac11-vpn-connected-window.png" alt="anyconnect connected window"
	style="margin:auto; width:75%; border:solid 1px black;" />

## FAQ

### VPNクライアントのインストールや接続時の問題

#### Q. 準備編 手順1で「これに対するアクセス権がありません」というエラーが表示される

- 多要素認証申請が完了していない可能性があります．[こちらのペー
ジ](https://utelecon.adm.u-tokyo.ac.jp/utokyo_account/mfa/)を参照して，
UTokyo Accountの多要素認証を有効にしてください．


#### Q. 準備編 手順2でダウンロードページが表示されず，真っ白なページが表示される


- [こちらのページ](https://vpn1.adm.u-tokyo.ac.jp/+CSCOE+/logon.html?tgroup=utvpn-tunnel-group)にアクセスしてダウンロードをお試しください．


#### Q. 準備編 手順2で「セッション管理データベースを更新できません」または「Unable to update the session management database」と表示されダウンロードページが表示されない

- 情報セキュリティ教育を受講していない可能性があります．情報セキュリティ
  教育を受講していない場合，UTokyo VPNは利用できません．対応については
  本部情報環境課セキュリティ対策チーム `jouhousecurity.adm __at__
  gs.mail.u-tokyo.ac.jp` (`__at__`を@に変更)にご自身のUTokyo Accountの
  ユーザ名を添えてご連絡ください．


#### Q. 利用編 手順4で「AnyConnect profile settings mandate a single local user, but multiple local users are currently logged into your computer. A VPN connection will not be established」というエラーが出て接続できない

- UTokyo VPNに接続しようとしている端末で複数ユーザが同時にログインして
  いる可能性があります．VPNに接続するユーザ以外はログオフしてください．


### 利用について

#### Q. 利用対象者は「UTokyo Accountを持つ本学教職員」とあるが，本学雇用者という事か．それとも，派遣職員や客員研究員等，本学で勤務または研究している者も含まれるか

- 派遣職員や客員研究員等，本学で勤務または研究している者も含まれます．


#### Q. 職員証発行や就労管理システムに学外からアクセスできるのか

- UTokyo VPNに接続することで学外から職員証発行や就労管理システムも利用
  可能です．


#### Q. 部局で管理している内部向けサイトは閲覧可能になるか

- 部局のサイトがどのようなアクセス制限をかけているかによるため，部局の
  サイト管理者にご確認ください．


#### Q. UTokyo WiFiのアカウントのように半年ごとに新規のアカウント取得は必要か

- UTokyo VPNの認証はUTokyo WiFiのアカウントではなくUTokyo Accountで行
  います．そのため基本的に利用者のアカウントの変更は起こらず，継続して
  利用が可能です．ただし，利用には年１回実施する情報セキュリティ教育の
  受講が必要です．


#### Q. 着任時には情報セキュリティ教育の受講期間が終了していた

- 着任時からUTokyo VPNを利用可能です．[情報セキュリティ教育](https://www.u-tokyo.ac.jp/adm/dics/ja/securityeducationvideo.html)のページにある「情報セキュリティ教育 教材」をよくお読みの上，ご利用ください．

#### Q. UTokyo VPN の利用申請は学外からも可能か

- 可能です．学内からは接続確認が難しい（本来学内で利用できるに学外から
  アクセスすることでVPNに接続できているか確認する必要があるため）ので
  学外での設定をお勧めします．


## 規定

- [UTokyo VPN利用規定](terms/UTokyoVPN-User-Term.pdf)
- [UTokyo VPN運用規定](terms/UTokyoVPN-Operation-Term.pdf)


## お問合せフォーム

お問合せはこちらの [UTokyo VPN問い合わせフォーム](https://forms.office.com/r/U0R5L40D3e) からお願いいたします．