# Privacy Policy for Pass For Now

_Last updated: 2026-04-20_

Pass For Now ("the app", "we", "us") is published by Articraftor LLC.
This policy describes what information the app
collects, where that information lives, and the choices you have
about it. It covers the current iOS release of Pass For Now.

If anything here is unclear, or you want to ask about something
specific, email us at support@articraftor.com — a human will reply.

---

## Summary (the short version)

- Almost everything Pass For Now stores about you stays on your
  device.
- We don't use analytics. We don't track you. We don't use
  advertising identifiers.
- Two third-party services are involved only when you use specific
  features: **RevenueCat** (for subscription state) and **Web3Forms**
  (for the in-app feedback form).
- We do not sell, rent, or share your information with anyone for
  advertising or marketing.

The rest of this page is the detail behind those bullet points.

---

## Information Pass For Now stores on your device

The app keeps the following on your phone, in local storage that
only the app itself can read:

- **Your onboarding answers** — the category, timing, channel, and
  trigger you selected, and the first-win and goal choices you made.
- **Your saves** — each logged "pass" event, with its amount,
  category, trigger, optional note, and timestamp.
- **App preferences** — notification time, reminder settings, and
  similar on/off choices.

This data is stored locally using
[`expo-sqlite`](https://docs.expo.dev/versions/latest/sdk/sqlite/) (a
SQLite database file inside the app's private iOS sandbox). Short
secrets the app needs — for example, the RevenueCat SDK key — are
stored in
[`expo-secure-store`](https://docs.expo.dev/versions/latest/sdk/securestore/),
which is backed by the iOS Keychain.

**We do not receive or read any of this data.** It never leaves your
phone unless you explicitly send a feedback message (see below).

If you uninstall Pass For Now, iOS deletes all of this data with the
app.

---

## Information that leaves your device

There are exactly two situations in which any information leaves
your phone. Both are opt-in in the sense that they only happen if
you take a specific action.

### 1. Subscription state — RevenueCat

If you start a free trial or purchase a Pass For Now Premium
subscription, we use [RevenueCat](https://www.revenuecat.com/) to
manage subscription state. RevenueCat is a third-party SDK that sits
between Pass For Now and Apple's StoreKit.

When you purchase or restore a subscription, the following is sent
to RevenueCat:

- A random, **anonymous** user identifier that the RevenueCat SDK
  creates on your device the first time the app launches. It is not
  derived from your Apple ID, your email, or any other personal
  information.
- The Apple transaction receipt Apple returns to the app after a
  purchase.
- Basic device metadata — OS version, app version, country code.

RevenueCat uses this information to:

- Verify your purchase with Apple.
- Tell the app whether you have an active **premium** entitlement.
- Match your purchase back to the same anonymous ID if you restore
  it on a new device.

We do **not** receive or store your Apple ID, your real name, your
payment information, or your credit card number. Apple handles
payment itself and never gives us that data.

RevenueCat's own privacy practices are at
https://www.revenuecat.com/privacy/.

### 2. Feedback messages — Web3Forms

Pass For Now forwards messages to our support inbox in two
situations, both using [Web3Forms](https://web3forms.com/) — a
third-party form-relay service:

- **When you submit the Send Feedback form** in Settings. The
  message text, and optionally your email, go to Web3Forms.
- **When you confirm subscription cancellation.** The
  **cancellation reason** you selected (e.g., "Too expensive")
  is forwarded along with any optional note you chose to write.
  You can cancel without this being sent only by closing the
  cancellation flow — if you tap "Manage in App Store" from the
  cancellation screen, your selected reason is forwarded.

The following information is sent to Web3Forms and then on to us:

- The **message text** you wrote (the optional note on the
  cancellation screen, or the feedback message in Settings).
- The **email address** you typed, if you included one (optional;
  only applicable to the Send Feedback form).
- The **cancellation reason** you selected, when submitting from
  the subscription-cancellation screen.
- Standard HTTP metadata that any web request includes — your IP
  address and your user-agent string. We do not read or store this
  metadata beyond the short time it takes Web3Forms to relay your
  message.

Web3Forms' privacy practices are at
https://web3forms.com/privacy-policy.

We keep feedback messages in our support inbox until we've replied
and a reasonable grace period has passed, after which we delete
them. If you'd like a specific message deleted sooner, email us at
**support@articraftor.com** with enough detail to identify it.

---

## Notifications

When you enable daily reminders, Pass For Now asks iOS for
permission to send you notifications. If you grant permission, we
schedule **local notifications only** — they live on your device,
fire at the risk time you set during onboarding, and never involve
a server. Nothing is tracked when a notification is delivered or
opened. You can turn reminders off at any time from **Settings →
Daily reminder** in the app, or from iOS Settings → Notifications
→ Pass For Now.

---

## What we do NOT do

- We do **not** use analytics services — no Google Analytics, no
  Mixpanel, no Amplitude, no PostHog, no Firebase Analytics, no
  in-house analytics pipeline. The app has an internal logger that
  writes to the on-device console only; we never see the output.
- We do **not** use the Apple advertising identifier (IDFA) and do
  not request App Tracking Transparency permission.
- We do **not** display third-party ads.
- We do **not** share, sell, rent, or trade your information with
  third parties for advertising or marketing purposes.
- We do **not** build a profile of you across other apps, websites,
  or services.
- We do **not** require an account. There is no sign-up, sign-in,
  password, or social login in Pass For Now.

---

## How long we keep data

- **On-device data:** for as long as you keep the app installed.
  You can wipe it at any time from **Settings → Reset Data**, or by
  uninstalling the app.
- **Subscription records at RevenueCat:** retained per RevenueCat's
  own retention policy (see their privacy page linked above), which
  generally keeps them for as long as the subscription is active
  plus a short period after cancellation.
- **Feedback messages in our support inbox:** until the issue is
  resolved plus a short grace period, then deleted.

---

## Your rights

Pass For Now doesn't have a backend account system, so you can
exercise most data-subject rights directly inside the app, with no
need to email us:

- **Access** — your saves and profile data are visible in the app's
  **History** and **Settings** screens.
- **Deletion** — **Settings → Reset Data** wipes every local record
  the app holds about you. Uninstalling the app also deletes it.
- **Correction** — edit your profile fields in **Settings → Your
  Profile**.
- **Subscription-record deletion** — to delete your RevenueCat
  subscription record, contact us at **support@articraftor.com**
  and we'll forward the request.

**California residents (CCPA / CPRA):** as of the date at the top of
this page we do not "sell" or "share" personal information as those
terms are defined in the California Consumer Privacy Act. If that
ever changes, we will update this page first.

---

## Children's privacy

Pass For Now is not directed at children under 13, and we do not
knowingly collect information from children under 13. If you believe
a child has used the app in a way that caused information to reach
us, contact **support@articraftor.com** and we will delete it.

---

## Region

Pass For Now is currently offered in the **United States**. If we
expand to additional regions we will update this policy to cover the
corresponding local requirements (GDPR for the EU, UK GDPR for the
UK, etc.) before we start distributing there.

---

## Changes to this policy

If we make material changes, we will update the **Last updated**
date at the top of this page. We recommend checking back
occasionally if you'd like to stay informed.

---

## Contact

**Pass For Now — Privacy**
Articraftor LLC
support@articraftor.com

---

_This policy is written in plain language on purpose. Nothing in it
is legal advice, and it isn't written in legalese because it doesn't
need to be._
