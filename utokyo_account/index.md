---
title: UTokyo Account
slug: utokyo_account # 手順を外部ファイルからincludeするときに使う
---

## UTokyo Accountとは
{:#about}

- **UTokyo Account**は，東京大学の情報システムを利用する際に必要となる全学的なアカウントです．東京大学の構成員（学生および教職員）が各種情報システムを利用する際は，このアカウントでサインインして利用することになります．
  - 現在アカウントを持っていない方でも，必要に応じてUTokyo Accountを発行することができることがあります．アカウントの発行を希望する場合は所属の学部・研究科等の窓口（学生は学務・教務担当，教職員は人事担当）にお問い合わせください．
- UTokyo Accountのユーザ名は10桁の数字で表され，**共通ID**とも呼ばれます．情報システム内では，`1234567890@utac.u-tokyo.ac.jp`のように，10桁の共通IDの後に東京大学であることを表す記号`@utac.u-tokyo.ac.jp`を付けたものが用いられることもあります．
  - 「10桁の共通ID＋`@utac.u-tokyo.ac.jp`」は通常利用できるメールアドレスではありません．
  - 「10桁の共通ID＋`@utac.u-tokyo.ac.jp`」に送られたシステムからの通知メールなどが[ECCSクラウドメール](/eccs_cloud_email)に転送されることがありますが，メールの送信には利用できません． 
- UTokyo Accountで利用できる情報システムについては，**[UTokyo Account Service Directory](https://login.adm.u-tokyo.ac.jp/utokyoaccount/)**や[「東京大学のシステム」のページ](/systems)をご覧ください．

## UTokyo Account利用上の注意
{:#notes}

1. UTokyo Accountは大学が組織的に受入し管理されている構成員に付与します．（大学が組織的に受入をしていない方には付与しません．）
1. UTokyo Accountで利用可能なサービスは利用者の身分・所属等により異なります．
1. UTokyo AccountおよびUTokyo Accountを利用する情報システムにおいては[情報倫理・コンピュータ利用ガイドライン](https://www.u-tokyo.ac.jp/content/400156696.pdf)を遵守してください．（参照：[東京大学情報セキュリティポリシー](https://www.u-tokyo.ac.jp/gen03/public16_j.html)）
1. UTokyo AccountおよびUTokyo Accountを利用する情報システムにおいて情報倫理・コンピュータ利用ガイドラインを遵守しない不適切な利用，安全性の問題を生じた場合はアカウントの停止をします．
1. UTokyo Accountの利用に際して必要な事項は本ページの情報を参照してください．

## UTokyo Accountを使い始めるには
{:#procedures}
{% include procedures/utokyo_account.html %}

以上の作業を終えたら，あわせて以下のページもご覧ください．

- 学生の方：「**[大学生活に必要な情報システムの準備について（新入生向け）](/oc/)**」
- 教員の方：以下の2ページをご確認ください．
    - 「**[東京大学における情報システムの準備について（教員向け）](/faculty_members/)**」
    - [UTokyo Portal「**UTokyo Accountの初期設定**」<small>（※閲覧にはUTokyo Accountでサインインする必要があります）</small>](https://univtokyo.sharepoint.com/sites/utokyoportal/wiki/d/UTokyo_Account_Initial_Settings.aspx)
- 職員の方：[UTokyo Portal「**UTokyo Accountの初期設定**」<small>（※閲覧にはUTokyo Accountでサインインする必要があります）</small>](https://univtokyo.sharepoint.com/sites/utokyoportal/wiki/d/UTokyo_Account_Initial_Settings.aspx)

## UTokyo Accountで情報システムにサインインする
{:#signin}

UTokyo Accountを用いるとさまざまな情報システムが利用可能です．状況により，サインイン方法が異なります．

- 以下の画面（安田講堂の画面）が表示された場合には，共通ID（数字10桁）とパスワードでサインインできます．
![](img/signin-yasuda.png)
- 安田講堂の画像が現れず，以下のようなサインイン画面が表示された場合には，「10桁の共通ID＋`@utac.u-tokyo.ac.jp`」を入力してください．
    <figure class="gallery">
        <img src="img/signin-utac-01.png">
        <img src="img/signin-utac-02.png">
    </figure>

なお，UTokyo Accountでサインインする情報システムの多くは互いに連携しており，最初にひとつの情報システムでユーザ名とパスワードを入力してサインインすると，それ以降に別の情報システムを利用する際にはユーザ名とパスワードの入力が不要になります．これを**シングルサインオン** (Single Sign-On, SSO) といいます．

## パスワードについて
{:#password}

### パスワードの有効期間
{:#password-expiration}

多要素認証を利用している場合は，パスワードに有効期限はありません．一方，多要素認証を利用していない場合，パスワードは変更してから397日（1年+1ヶ月）間有効です．現在のパスワードの有効期限は，[利用者メニュー](https://utacm.adm.u-tokyo.ac.jp/webmtn/LoginServlet)から確認することができます．

<div class="box">
※以前は，多要素認証を利用しているかどうかにかかわらず，パスワードの有効期間は365日でした（<a href="/notice/2023/03-utokyo_account-password">詳細はこちら</a>）．変更日である2023年3月9日までに設定したパスワードの有効期間は365日のままで延長されておらず，同日以降に設定したパスワードから新しい有効期間になっています．
</div>

### パスワードを変更する
{:#change-password}

[利用者メニュー](https://utacm.adm.u-tokyo.ac.jp/webmtn/LoginServlet)内の「パスワードの変更」から，パスワードを変更することができます．なお，パスワードの有効期限が切れた場合でもパスワードの変更は可能で，パスワードの再設定や再発行をする必要はありません．

### パスワードを忘れた場合
{:#forget-password}

UTokyo Accountのパスワードを忘れた場合には，次のような手順を踏むことでアカウントに再びサインインすることができます．

#### メールでパスワードを再設定する
{:#reset-password}

人事情報MyWeb（教職員）やUTAS（学生）で事前にメールアドレスを登録している場合には，そのメールアドレスを利用してパスワードを再設定することができます．具体的には，以下の場所で設定されているメールアドレスが使用されます．

- 学生の場合：<a href="https://utas.adm.u-tokyo.ac.jp/campusweb/campusportal.do">UTAS</a>の「学生情報」メニューにある「現住所等変更入力」の「E-MAIL 1」欄（なお，「E-MAIL 2」のアドレスは再設定用のメール送信先としては使えません）
    - 学部1年生の新入生の場合，[合格発表の際に情報登録を行ったWebシステム](https://utas-ew.adm.u-tokyo.ac.jp/)に登録していたメールアドレスが自動で設定されています．
- 教職員の場合：<a href="https://univtokyo.sharepoint.com/sites/utokyoportal/wiki/d/Personal_information_and_ID_card.aspx">人事情報MyWeb</a>の「パーソナルメニュー」にある「本人属性変更：登録画面」の「学内メールアドレス」欄

再設定の手順は以下の通りです．

1. 「[UTokyo Account パスワード再設定](https://utacm.adm.u-tokyo.ac.jp/webmtn/multi/jpn/reset.html)」下部の「パスワード再設定」を押してください．
1. 「メールまたはユーザ名」の欄に「10桁の共通ID＋`@utac.u-tokyo.ac.jp`」を，その下の欄に画像の文字を入力してから「次へ」を押してください．
1. 事前に登録されているメールアドレスの一部分が表示されているので，確認してください．このメールアドレスに，パスワードを再設定するために必要な確認コードが書かれた通知メールが届きます．
1. 通知メールが届いたら，メールの指示に従って再設定の手続きを行ってください．メールが届かない場合には，迷惑メールフォルダなどに紛れ込んでいないかどうか，違うメールアドレスを見ていないかを確認してください．

<details>
	<summary>「パスワードのリセットを登録していないため、自分でパスワードをリセットすることはできません」と表示され，再設定ができない場合</summary>
	システムにメールアドレスが登録されていないため，通知メールを送信することができず，したがってパスワードの再設定ができません．<a href="#reissue-password">窓口でパスワードを再発行</a>してください．
	パスワードを再発行することができたら，メールアドレスをUTAS（学生）や人事情報MyWeb（教職員）に登録してください．
</details>

#### 窓口でパスワードを再発行する
{:#reissue-password}

メールアドレスを未登録の場合や，上記の手順がうまくいかない場合には以下の窓口でパスワードを再発行してください．

- 所属する学部・研究科等の学務・教務担当窓口（学生のみ）
    - 学生証を持参してください．
    - 学部1年生の新入生の方で，まだ学生証を受け取っていない場合は，合格通知書を持参してください．
- 所属する部局の人事担当（教職員のみ）
- [ECCS窓口](https://www.ecc.u-tokyo.ac.jp/map.html)
    - 学生は学生証，教職員は職員証を持参してください．
    - 窓口は，情報教育棟（駒場キャンパス），情報基盤センター（本郷地区浅野キャンパス），福武ホール（本郷キャンパス）に設置されています．

手続きを行うと，初期パスワードが記載された「パスワード通知書」が発行されます．「[UTokyo Accountを使い始めるには](#procedures)」の「作業：初期パスワードを変更する」を参考に，初期パスワードを新しいものに変更してください（初期パスワードのままでは，各種情報システムを利用することができません）．

## 多要素認証 (MFA)
{:#mfa}

UTokyo Accountでは**多要素認証** (Multi-Factor Authentication, MFA) を導入しています．多要素認証を設定すると，アカウントにサインインする際に，パスワードに加えて，SMSや専用のアプリ等での本人確認が要求されるようになります．詳細は[UTokyo Accountにおける多要素認証の利用について](mfa/)を参照してください．
