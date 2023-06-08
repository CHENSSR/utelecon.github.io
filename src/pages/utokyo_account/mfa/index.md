---
title: UTokyo Accountにおける多要素認証の利用について
---

<div class="box--alert">
【お知らせ】<a href="/notice/2023/02-utokyo_account-security">2月27日から「Microsoft Authenticator」アプリのサインイン承認手順が変わります</a>
</div>

## はじめに
{:#introduction}

東京大学の情報システムのセキュリティ向上を目的として，UTokyo Accountに多要素認証を導入しています．

多要素認証 (Multi-Factor Authentication, MFA) とは，アカウントへのサインイン時に，パスワードに加えて，SMSや専用のアプリなどで本人確認を行う認証方法です．多要素認証を利用すると，なんらかの事情でパスワードが他人に知られた場合でも，アカウントにサインインされる可能性を低くすることができ，セキュリティを向上することができます．

UTokyo Accountでは，利用者が各自で初期設定を行うことにより，多要素認証の利用が有効化されます．現時点においては多要素認証の利用は必須ではなく，基本的には多要素認証を利用しなくてもUTokyo Accountの利用は可能ですが，セキュリティの観点からは**多要素認証の利用を強く推奨**します．ただし，**[UTokyo VPN](/utokyo_vpn/)および[UTokyo Slack](/slack/)の利用には多要素認証の有効化が必須**となっており，多要素認証を有効化していない場合は利用できません．

UTokyo Accountのセキュリティを確保することは，利用者個人の情報だけなく，大学が保有する情報資産を守るために非常に重要ですので，多要素認証を利用していただくようご協力をお願いいたします．

## 多要素認証の初期設定（利用開始）

多要素認証の初期設定手順（利用を開始するための手順）は，以下のページを参照してください．

<b class="box center"><a href="initial">UTokyo Account多要素認証の初期設定手順</a></b>

## 故障や機種変更などで本人確認ができずサインインできなくなった場合

故障や機種変更などで本人確認方法（スマホアプリや電話番号）が使えなくなり，そのために多要素認証によるサインインができなくなった，という場合，以下のページを参照して対応してください．

<b class="box center"><a href="reregister_and_terminate">多要素認証の本人確認方法再登録および利用終了について</a></b>

なお，機種変更の際は，古いスマホが利用できるうちに「[UTokyo Account多要素認証の本人確認方法の登録変更手順](change)」に従って新しいスマホを追加登録しておくことで，UTokyo Accountにサインインできないという事態を避けることができます．必ず事前に登録変更を行うようにしてください．

## その他
{:#others}

以上のほか，多要素認証の利用に関する説明は項目ごとに分けて説明しています．以下より目的のページを開いてください：

- **[本人確認方法の登録変更手順](change)**：多要素認証の本人確認方法（スマホアプリや電話番号）を変更する手順について説明します．
    - [本人確認方法を追加する](change#add)
    - [既定（デフォルト）の本人確認方法を変更する](change#default)：複数の本人確認方法のうち，毎回のサインイン時に最初にどれが提示されるか設定します．
    - [設定済みの本人確認方法を変更する](change#edit)
    - [本人確認方法を削除する](change#delete)
- **[多要素認証の利用を終了する](reregister_and_terminate)**：多要素認証の利用をやめてパスワードだけでサインインできる状態に戻す手続きです．セキュリティの観点から多要素認証を利用することを推奨しておりますが，やむを得ない事情がある場合には利用終了手続きを受け付けています．
- **[その他](others)**
    - [ハードウェアトークンの貸出について（教職員向け）](others#hardware-token)：スマートフォンを持っていないなどの理由で本人確認方法が登録できない教職員向けに，代わりに本人確認方法として登録できる「ハードウェアトークン」という専用の機器の貸出について説明します．
    - [Microsoft Authenticatorで6桁のコードを使ってサインインする方法](others#msauth-totp)：本人確認方法として「Microsoft Authenticator」アプリを登録した場合に，通知を受け取る標準的な手順とは異なる手順で本人確認を行う方法について説明します．
    - [サインイン時の本人確認の挙動について](others#irregular)
    - [「不明なエラーが発生しました」エラーについて](others#unknown-error)：サインイン画面で「不明なエラーが発生しました」と表示された場合，こちらの説明に従ってください．

<!--

## 故障や機種変更などで本人確認ができずサインインできなくなった場合
{:#troubleshooting}

故障や機種変更などで本人確認方法が使えなくなったため多要素認証によるサインインができなくなった，という場合の対処法を説明します．

なお，**対処を済ませサインインできるようになったら，設定を変更して複数の本人確認方法を使える状態にしておくことを強く推奨します**．上の「[多要素認証の設定変更手順](#change)」で説明しているとおり，[多要素認証の設定ページ](https://mysignins.microsoft.com/security-info?domain_hint=utac.u-tokyo.ac.jp)から設定を変更してください．

### 他の本人確認方法を使う
{:#troubleshooting-alternative}

登録済みの他の本人確認方法が使える状態であれば，それを使ってサインインすることができますので，まずはそれを試してください．

サインイン時（パスワード入力後）に表示される本人確認を行う画面で，「問題がありますか? 別の方法でサインインする」あるいは「別の確認オプションを使用する」というリンクを探して押してください．
<img src="signin_with_another_method.png">
デフォルト（自動的に選ばれるもの）以外のものも含め，設定済みの本人確認方法が一覧で表示されます．

- この中に使える状態の本人確認方法があれば，それを選んでその方法で本人確認を行うことで，UTokyo Accountにサインインすることができます．
- 表示された本人確認方法がすべて使えない状態であれば，本人確認方法の再登録手続きを行う必要があります．次の「本人確認方法を再登録する」の説明に進んでください．

### 本人確認方法を再登録する
{:#troubleshooting-reregister}

登録済みの本人確認方法がすべて使えない状態となってしまった場合は，本人確認方法の再登録手続きを行う必要があります．「**[UTokyo Account多要素認証の本人確認方法再登録および利用終了について](reregister_and_terminate)**」のページを参照してください．

## その他
{:#others}

### 多要素認証の申請を取り消したい・多要素認証の利用を終了したい
{:#others-terminate}

セキュリティの観点から多要素認証を利用することを推奨しておりますが，やむを得ない事情がある場合には，多要素認証の利用を終了し，パスワードだけでサインインできる状態に戻すことができます．「**[UTokyo Account多要素認証の本人確認方法再登録および利用終了について](reregister_and_terminate)**」のページを参照してください．

なお，多要素認証の本人確認方法が利用できずサインインできなくなったという場合は，上の「[多要素認証の本人確認ができずサインインできなくなった場合](#troubleshooting)」で説明しているとおり，「本人確認方法の再登録」を行うことによりサインインできるようになりますので，多要素認証の「利用終了」をする必要はありません．

-->