---
title: UTokyo Wi-Fi
slug: utokyo_wifi
---

<div class="box--alert box--important">
[Important] <a href="/en/notice/2023/01-wifi">Changes in usage of UTokyo Wi-Fi due to renewal</a>
</div>

## About UTokyo Wi-Fi

UTokyo Wi-Fi is a Wi-Fi service available to members of the University of Tokyo for educational and research purposes. Currently, UTokyo Wi-Fi is available in most classrooms on the Hongo, Komaba, Kashiwa, and other campuses. Please refer to the [Caution](#caution-to-use) before using UTokyo Wi-Fi.


## Before using UTokyo Wi-Fi

### Availabilities

- UTokyo Wi-Fi is available to members of the University of Tokyo (students & faculty and staff members) who have a [UTokyo Account](/en/utokyo_account/).
  - If you have not completed the Information Security Education course, your access may be suspended even if you are a member of the University of Tokyo. Please refer to the "[Information Security Education](#jouhou-security)" section below for more details.
- In order to use UTokyo Wi-Fi, UTokyo Wi-Fi Account is required for each semester in addition to your UTokyo Account.


### Caution
{:#caution-to-use}
1. UTokyo Wi-Fi is available only for the University’s education and research, as well as the business activities stipulated by the National University Corporation Act.
2. UTokyo Wi-Fi is available to those who have agreed to the "[Terms of Use for the University of Tokyo Wireless Network System (UTokyo WiFi)](https://www.u-tokyo.ac.jp/adm/dics/ja/wifi_termsofuse.html)" and have applied to use the service.
3. Only the applicant is allowed using UTokyo Wi-Fi. The account must not be lent to others. Please manage your so it will not be abused.
4. UTokyo Wi-Fi will monitor communications and restrict access to sites supposedly inappropriate to ensure information security.
5. UTokyo Wi-Fi account will be suspended when "[Terms of Use for the University of Tokyo Wireless Network System (UTokyo WiFi)](https://www.u-tokyo.ac.jp/adm/dics/ja/wifi_termsofuse.html)" are violated. (e.g. failure to attend the Information Security Education specified by the university)
6. Please deal with a security incident immediately when you receive a notification for it while using UTokyo Wi-Fi.
7. UTokyo Wi-Fi is provided for those who can set up their own devices by themselves.
8. UTokyo Wi-Fi usage data may be disclosed to the public for the purposes of the university administration with the statistical process to make individuals not identified.

### Information Security Education
{:#jouhou-security}

The University of Tokyo conducts annual [Information Security Education](https://www.u-tokyo.ac.jp/adm/dics/ja/securityeducationvideo.html) for all UTokyo Account holders. The beginning of the course will be notified (May for students and July for faculty and staff in the case of FY2022), so please be sure to take the course. **Failure to complete the course will result in suspension of your UTokyo Wi-Fi privileges until the end of that academic year, and you will not be able to connect to UTokyo Wi-Fi.** Once your account is suspended, you will not be able to log in to the account menu or create a new account.


<details>
	<summary>If the course registration period has ended at the time of arrival or enrollment in the university</summary>
	In this case, your UTokyo Wi-Fi Account will not be suspended, and you will be able to use UTokyo Wi-Fi from the time of your arrival or enrollment. Please read carefully the "Information Security Education Materials" on the Information Security Education page before you start using UTokyo Wi-Fi. Information security education is provided every year, so please take the course from the next year onward.

</details>
<details>
	<summary>If you have failed to complete information security training by the prescribed time </summary>
  The UTokyo Wi-Fi account will be suspended for the current year, so basically you will not be able to use UTokyo Wi-Fi until the end of the fiscal year. For more information on thepeople who have not yet taken the course, please contact <code>jouhousecurity.adm__at__gs.mail.u-tokyo.ac.jp</code> (<code>__at__</code> transfer to @) with your UTokyo Account username (10-digit common ID).
</details>

### Using UTokyo Wi-Fi on Shared Devices
UTokyo Wi-Fi is only available on individuals' own device: **it is prohibited to use UTokyo Wi-Fi on a shared device by more than one person.** Because it allows anyone other than the user who owns a UTokyo Wi-Fi Account to use the service, and it is considered to be lending of an account, which is prohibited by the Terms of Use. However, if the OS user account is set up separately for each individual, and the UTokyo Wi-Fi account can only be used by the person who has obtained it, UTokyo Wi-Fi is able to be used.

## Steps to start using the service
{:#initial-setup}

<ul class="gap">
  <li>
    <strong>Step 1: Check the devices to be used </strong>
    <div>Laptops, smartphones, and tablets can generally connect to UTokyo Wi-Fi. However, other types of electronic devices and older devices may not be able to connect. For example, devices that do not support WPA2-Enterprise cannot be connected. Please check for updates to the OS and drivers of your devices and update them appropriately before connecting to UTokyo Wi-Fi.</div>
  </li>
  <li>
    <strong>Step 2: Apply for a UTokyo Wi-Fi Account</strong>
{% include en/systems/utokyo_wifi/apply.html %}
  </li>
  <li>
    <strong>Step 3: Connect to UTokyo Wi-Fi</strong>
{% include en/systems/utokyo_wifi/connect.html %}
  </li>
</ul>


## Information on usage
### Account expiration date
{:#expiration}

UTokyo Wi-Fi accounts expire at the end of April of the following fiscal year. New accounts can be issued before the start of each fiscal year, so if you want to continue using UTokyo Wi-Fi, you need to reissue an account each fiscal year.

- The procedure for reissuing an account is the same as Steps 2 and 3 above.
    - If you have not taken the information security training course and your account has been suspended, you cannot reissue an account. Please refer to the "[Information Security Education](#jouhou-security)" section above for details.
- Once the account has been reissued, enter the user ID and password for the new account into the device you use and connect to it.
    - If the device remembers your previous UTokyo Wi-Fi account information and you are not able to change it (i.e., screen to enter a new user ID and password does not appear), please delete your Wi-Fi account information on the device. The specific method of the removal varies depending on the OS and device type, so please refer to the manual of the respective device. For Windows, please also refer to [ECCS Tutor's Page](https://www.sodan.ecc.u-tokyo.ac.jp/en/faq/utokyo-wifi-win10-en/), and for iOS, please refer to the official help "[How to forget a Wi-Fi network on your iPhone, iPad, iPod touch, or Mac](https://support.apple.com/en-us/HT208941)".

### Connect Configuration
{:#connect-configuration}

<table>
  <tr>
    <th>SSID</th> <td><code>0000UTokyo</code><div>* The old SSID <code>UTokyo-WiFi</code> used before <a href="/en/notice/2023/01-wifi">the update</a> is gradually becoming unavailable.</div></td>
  </tr>
  <tr>
    <th>Security</th> <td>WPA2-Enterprise (802.1X)</td>
  </tr>
  <tr>
    <th>Encryption</th> <td>CCMP (AES)</td>
  </tr>
  <tr>
    <th>Authentication Method</th> <td>PEAP MSCHAPv2 (EAP-MSCHAPv2)</td>
  </tr>
  <tr>
    <th>Server Certificate</th>
    <td>
      <ul style="margin-top: 0; margin-bottom: 0;">
        <li>Name (Common Name): <code>acm.wifi.adm.u-tokyo.ac.jp</code></li>
        <li>Issued by: <code>NII Open Domain CA - G7 RSA</code></li>
        <li>Root Certificate: <code>Security Communication RootCA2</code></li>
        <li>Fingerprint SHA-1: <code style="word-break: break-all;">6D:F0:B1:18:F1:8F:16:A5:D3:94:AC:E2:26:7A:C1:0A:F2:94:B1:37</code></li>
        <li>Fingerprint SHA-256: <code style="word-break: break-all;">6F:CF:A6:06:B1:45:C2:23:53:E7:BA:D7:B4:08:B3:CD:22:DA:80:A0:1A:6A:E3:91:9A:3A:47:E6:C0:6A:AB:46</code></li>
      </ul>
      * If you are prompted to enter the "domain" of the certificate, enter <code style="word-break: break-all;">u-tokyo.ac.jp</code>.</td>
  </tr>
</table>

### Security measure

The network of UTokyo, including UTokyo Wi-Fi, is secured by UTokyo Campuswide Firewall and other measures to ensure information security.
- Some websites cannot be viewed over UTokyo Wi-Fi because they are blocked by UTokyo Campuswide Firewall.
- UTokyo WiFi Task Force or the staff of your department (Department CERT) may contact the user by email if it detected communication that may cause a security problem.
    - The e-mail addresses of UTokyo WiFi Task Force are `utokyo-wifi-cert.adm_at_gs.mail.u-tokyo.ac.jp` or `utokyo-wifi-tf_at_itc.u-tokyo.ac.jp` (please read `_at_` as @).
    - Failure to respond to the email may result in account suspension. In order to reactivate a suspended account, you must consult with your department’s CERT and take reasonable steps to prevent a recurrence.

## Others

- There is no limit to the number of devices per account that can be connected to UTokyo Wi-Fi.
- You cannot delete your UTokyo Wi-Fi account directly. However, you can make it invalid with reissuing a new account by clicking the "New Application" button in the "UTokyo Wi-Fi Account Menu".
- Please note that UTokyo Wi-Fi may become temporarily unavailable in certain locations or throughout the campus due to trouble. We apologize for any inconvenience, and we will make efforts to deal with the problem quickly.
- In addition to UTokyo Wi-Fi, the University of Tokyo has other wireless LAN services that are available on campus. All members of and visitors to the University of Tokyo are requested to refer to [the WiFi services in UTokyo](https://www.u-tokyo.ac.jp/adm/dics/ja/wlan.html) page before using UTokyo Wi-Fi and use the service appropriately.
  - You will be able to use UTokyo Wi-Fi account user ID and password to connect to [eduroam](https://eduroam.jp/en), a wireless LAN service that allows mutual use among universities and research institutions.
    - Only UTokyo Wi-Fi accounts issued after January 31, 2023 will be eligible for this.
- If you are in charge of a network of your department,  please also refer to [the Information on UTokyo Portal](https://univtokyo.sharepoint.com/sites/utokyoportal/wiki/d/UTokyo_WiFi_Management.aspx).

## Troubleshooting and Inquiries

If you encounter any problems when using the system, please check the following points first.
- If you are having problems connecting for the first time, carefully reread the "[Steps to start using the service](#initial-setup)" section of this page. Also, please refer to the [ECCS Tutor's Page](https://www.sodan.ecc.u-tokyo.ac.jp/en/faq/utokyo-wifi-en/), which contains detailed connection instructions for each device as necessary.
- If you encounter problems on the second or subsequent connections, please refer to "[Account expiration date](#expiration)" on this page.
- Please consult with your friends, colleagues, and others around you who already succeeded in connecting.

If you still have trouble, please contact **[Technical Support Desk](/en/support)**. Please understand the following points when making inquiries.
- We receive many inquiries. In most cases, it is difficult to respond immediately.
- We cannot always provide support for a specific model because it is impractical to possess and test all types of equipment. Please consider contacting the distributor or manufacturer.

[ECCS Tutors](https://www.sodan.ecc.u-tokyo.ac.jp/en/), the student staff, are located at several places on campus and available for face-to-face, in-person consultation.


