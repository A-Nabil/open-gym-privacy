---
title: Privacy Policy — Open Gym
permalink: /
---

# Privacy Policy — Open Gym

**Effective date:** 30 April 2026
**Last updated:** 30 April 2026

This Privacy Policy explains how the **Open Gym** mobile application
(package name `com.opengym.app`, the "App") collects, uses, and protects your
personal data. The App is published on Google Play by **Ahmed Nabil**, an
individual developer based in **Sweden**.

For the purposes of the EU General Data Protection Regulation
(Regulation (EU) 2016/679, "GDPR") and the Swedish Data Protection Act
(*Lag (2018:218) med kompletterande bestämmelser till EU:s
dataskyddsförordning*), the **data controller** is:

> **Ahmed Nabil**
> Sweden
> Contact: **a.nabil.abdalah@gmail.com**

If you have questions about this policy or wish to exercise any of your
rights described below, please contact us at the email above.

---

## 1. Summary

Open Gym is a personal fitness companion. It generates personalised workout
and nutrition plans based on profile information you enter during
onboarding. To keep things short, here is the high-level picture:

- The App **does not require an account**. There is no sign-up, no login,
  no email or password, and no user profile stored on our servers.
- The App **does not show advertising** and does not contain any
  advertising SDKs.
- The App **does not include any third-party analytics, crash reporting,
  or tracking SDKs** (no Firebase, no Google Analytics, no Crashlytics,
  no Facebook SDK, no Mixpanel, etc.).
- Your fitness profile (age, height, weight, goals, dietary preferences,
  workout history, meal logs) is stored **on your device** in an
  **encrypted local database** (SQLCipher).
- When you ask the App to generate a plan, your profile inputs are
  transmitted to our Azure-hosted backend to produce the plan and are
  **not retained by us** beyond what Microsoft Azure keeps in standard
  server logs for operational and diagnostic purposes.

The sections below explain each point in detail.

---

## 2. Data we collect

### 2.1 Information you provide during onboarding

To generate accurate workout and nutrition plans, the App asks you for:

- Age
- Gender
- Height and weight (and target weight, if you set one)
- Activity level
- Workout experience level
- Primary fitness goal (e.g. lose weight, build muscle, keep fit, get
  stronger)
- Optional target date for your goal
- Dietary restrictions (e.g. halal, vegetarian, vegan, gluten-free)
- Cooking skill level
- Workout and meal preferences (which exercises and meals you log,
  whether you choose to track workouts, etc.)

This information is **fitness-related personal data**. Some of it (height,
weight, dietary information) may be considered **health-related data**
under Article 9 GDPR. We process it on the legal basis of your
**explicit consent** (Article 9(2)(a) GDPR), which you give by entering
the information into the App. You can withdraw your consent at any time by
deleting the data from within the App, by uninstalling the App, or by
contacting us.

### 2.2 Information stored locally on your device

The following are stored only on your device, in an encrypted local SQLite
database (using SQLCipher) and in Android shared preferences /
secure storage:

- Your onboarding answers (above)
- Your workout history (which workouts you completed, when, and any logged
  weights/reps)
- Your meal logs
- Your notification preferences
- App settings (language, theme)

We do **not** receive copies of your workout or meal history. They live on
your device until you delete them or uninstall the App.

### 2.3 Information transmitted to our backend

When you request a workout or nutrition plan, the App sends a subset of
your onboarding data to our backend at
`https://open-gym-backend.azurewebsites.net` so it can generate the plan.
The legal basis for this processing is **performance of a contract**
(Article 6(1)(b) GDPR) — providing the plan you requested — and your
**explicit consent** for any health-related fields (Article 9(2)(a)).

We **do not maintain user accounts or persistent user profiles**. The
profile data submitted during plan generation is used to produce the
response and is **not stored by us** beyond what Microsoft Azure retains
in standard server logs (request timestamps, IP addresses, and request
metadata) for operational and diagnostic purposes. Azure log retention
follows Microsoft's defaults; we do not extract or analyse personal data
from those logs.

### 2.4 Approximate location (country only)

To set a sensible default language and to localise plan content, the App
makes a single request to the public IP-geolocation service
**`freeipapi.com`** to determine the **country** associated with your
device's IP address. We do **not** use GPS, Wi-Fi, or any
device-location permission, and we do not collect city, region, or
precise coordinates. The request is made by your device directly to
`freeipapi.com`; we do not store the result on our servers.

### 2.5 Permissions the App requests on Android

| Permission | Why |
|---|---|
| `INTERNET`, `ACCESS_NETWORK_STATE` | To call our backend and load exercise videos/images |
| `POST_NOTIFICATIONS` | To send local workout and meal reminders you schedule |
| `VIBRATE` | To vibrate the device when a notification fires |
| `RECEIVE_BOOT_COMPLETED` | To re-register your scheduled local notifications after the device restarts |

The App does **not** request location, camera, microphone, contacts, SMS,
calendar, or photo permissions.

---

## 3. Third-party services

The App connects to the following third-party services. We have no
control over the data practices of these providers. We recommend you
read their privacy policies if you have concerns.

### 3.1 Microsoft Azure (data processor)

Our backend runs on **Microsoft Azure Functions** (region:
West Europe). When you generate a plan, your profile inputs are
transmitted to Azure to be processed. Microsoft acts as our **data
processor** under Article 28 GDPR. See Microsoft's Data Protection
Addendum and privacy statement at
<https://privacy.microsoft.com/en-us/privacystatement>.

### 3.2 YouTube (Google LLC)

The App embeds YouTube videos to demonstrate exercises, using Google's
official `youtube_player_flutter` plugin and the standard YouTube
embedded player. When you watch a video, **Google may collect data
about your interaction** (e.g. cookies, viewing history) according to
Google's Privacy Policy at <https://policies.google.com/privacy> and
the YouTube Terms of Service at <https://www.youtube.com/t/terms>. We
do not receive this data.

### 3.3 Google Fonts (Google LLC)

The App downloads typography (the "Inter" and "Space Grotesk" font
families) from **Google Fonts** (`fonts.googleapis.com`) on first
launch and caches them locally. The request includes your IP address.
See <https://policies.google.com/privacy>.

### 3.4 freeipapi.com

Used to detect your country from your IP address (see section 2.4). See
<https://freeipapi.com/>.

### 3.5 musclewiki.com (exercise images)

Some exercise illustrations are loaded from
`media.musclewiki.com` and cached locally for performance.

---

## 4. Advertising and analytics

The App contains **no advertising**, **no in-app purchases**, **no
subscriptions**, and **no third-party analytics or tracking SDKs**. We
do not build advertising profiles. We do not share your data with
advertising networks. We do not use cookies inside the App.

The only analytics signals available to us are the standard server logs
that Microsoft Azure produces for operational reasons (see section 2.3).

---

## 5. Children

The App is **not directed at children under 13** and we do not knowingly
collect personal data from children under 13. The recommended Play Store
target audience for the App is **13 and older**. If you believe a child
under 13 has used the App and provided personal data, please contact us
at the email above and we will take reasonable steps to delete the data.

For users in the European Union, the App is intended for users aged
**16 and older** in line with Article 8 GDPR. Member States may set a
lower age (down to 13); please follow the rules that apply where you
live.

---

## 6. How we keep your data secure

- The on-device fitness database is **encrypted with SQLCipher**.
- Sensitive configuration values are stored in **Android Keystore /
  iOS Keychain** via the `flutter_secure_storage` plugin.
- All network traffic uses **HTTPS (TLS)**.
- Our backend is hosted on Microsoft Azure, which provides
  industry-standard infrastructure security.

No method of electronic transmission or storage is 100 % secure;
however, we apply reasonable technical and organisational measures
proportionate to the risks of the limited data we process.

---

## 7. Data retention

- **On-device data:** retained until you delete it from within the App,
  clear the App's data in Android settings, or uninstall the App.
- **Backend processing:** plan-generation requests are not stored as
  user records. Standard Azure server logs are retained according to
  Microsoft's defaults (typically up to 90 days for diagnostic logs).
- **Email correspondence with us:** retained for as long as needed to
  handle your request, typically up to 12 months, then deleted unless
  retention is required by law.

---

## 8. International data transfers

Our backend runs in the European Economic Area (Microsoft Azure West
Europe). YouTube, Google Fonts, and freeipapi.com may process your IP
address outside the EEA. Where personal data is transferred outside the
EEA, the recipient relies on safeguards such as the **EU Standard
Contractual Clauses** and (for Google) the **EU–US Data Privacy
Framework**.

---

## 9. Your rights under the GDPR

If you are in the European Union, the European Economic Area, the
United Kingdom, or Switzerland, you have the following rights:

- **Right of access** (Article 15) — request a copy of any personal
  data we hold about you.
- **Right to rectification** (Article 16) — ask us to correct
  inaccurate data.
- **Right to erasure / "right to be forgotten"** (Article 17) — ask us
  to delete your data. (Note: most data lives only on your device and
  you can delete it directly in the App.)
- **Right to restriction of processing** (Article 18).
- **Right to data portability** (Article 20).
- **Right to object** (Article 21).
- **Right to withdraw consent** at any time (Article 7(3)), without
  affecting the lawfulness of processing prior to withdrawal.

To exercise any of these rights, email us at
**a.nabil.abdalah@gmail.com**. We will respond within one month, as
required by Article 12(3) GDPR.

You also have the right to **lodge a complaint with a supervisory
authority**. In Sweden this is the *Integritetsskyddsmyndigheten*
(IMY): <https://www.imy.se/>. You may also contact the supervisory
authority in your own country of residence.

---

## 10. Account deletion

The App does not have user accounts, so there is no separate
"delete account" step. To delete all data the App has stored about you:

1. Open the App.
2. Use the in-app option to clear your profile and history, **or**
3. Uninstall the App, **or**
4. In Android Settings → Apps → Open Gym → Storage → "Clear data".

If you wish to be sure that no residual data remains in our backend
logs, email us at **a.nabil.abdalah@gmail.com** and we will request
log deletion from Microsoft Azure on your behalf to the extent
operationally possible.

---

## 11. Changes to this policy

We may update this policy from time to time. The "Last updated" date
at the top of the page reflects the current version. Material changes
will be communicated through an in-app notice or via the Google Play
listing.

---

## 12. Contact

For any privacy-related question or to exercise your rights, contact:

**Ahmed Nabil**
Email: **a.nabil.abdalah@gmail.com**
Country: Sweden
# open-gym-privacy
Privacy policy for the Open Gym mobile app
