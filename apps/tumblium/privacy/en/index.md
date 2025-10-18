---
layout: default
title: Tumblium Privacy Policy
description: Privacy policy for the Tumblium app
lang: en
---

# Privacy Policy (Tumblium)

Last Updated: 2025-10-18

This privacy policy (the “Policy”) describes how Tumblium (the “App”) handles user information.

Before using the App, please read this Policy carefully.

Language: English | [日本語](/apps/tumblium/privacy/)

Note: If there is any inconsistency between translations, the Japanese version prevails.

## 1. Information We Collect

Depending on the features in use, the App may collect the following information:

- Minimal settings/state required for app functionality (stored on device only)
- Crash reports and diagnostics (only if the user opts in)
- Identifiers/tokens from external services when explicitly linked by the user

## 2. How We Collect Information

- Information you enter or actions you take in the App
- Information provided via device/OS APIs
- Data sent by crash/analytics SDKs when explicitly enabled by the user

## 3. Purposes of Use

We use collected information for the following purposes:

- Provide, maintain, protect, and improve the App
- Investigate issues and improve performance
- Inform decisions on new features and improvements
- Provide user support when necessary

## 4. Storage and Sharing

- Data stored on the device is not transmitted externally except when you explicitly perform an action or provide consent.
- If crash/analytics is enabled, data may be sent to the service provider (e.g., platform diagnostics or analytics services).
- We do not sell personal information to third parties. Disclosure occurs only when legally required or to protect life and property in emergencies.

### Data Stored On Device

- Dashboard cache: latest ~20 posts (for faster startup rendering)
- Read history: IDs of posts you have read (to show read/unread)
- Scroll position: last viewed position in the feed
- OAuth tokens: for Tumblr API access (stored in Keychain/Secure Storage)
- Image cache: temporary image cache via SDWebImage

All of the above remain on your device; nothing is sent to our own servers.

## 5. Third Party Disclosure

We do not disclose personal information to third parties except in the following cases:

- When legally required by law
- To protect life, body, or property when obtaining user consent is difficult
- When necessary for business operations within appropriate contractual and management frameworks

## 6. Tumblr Integration (Required)

The App is a Tumblr client. All features are provided through the Tumblr API.

- Authentication: OAuth 2.0 with PKCE
- Data obtained: Tumblr dashboard, likes, your posts, user profile, etc.
- Data sent to Tumblr: user actions such as like, reblog, delete, etc.
- Data retention: data tied to your Tumblr account is managed by Tumblr
- Privacy: subject to Tumblr’s Privacy Policy (https://www.tumblr.com/policy/privacy)

### Other External Services (General)

If the App integrates services other than Tumblr, such integrations follow each provider’s terms. Enablement requires explicit user action/consent. Details will be added here when finalized.

### External Services / SDK List (Tumblium)

{% assign sdks = site.data.policies.tumblium.sdks %}
{% if sdks and sdks.size > 0 %}
<ul>
{% for s in sdks %}
  <li>
    <strong>{{ s.name }}</strong>
    {% if s.provider %}(Provider: {{ s.provider }}){% endif %}<br>
    Purpose: {{ s.purpose | default: '—' }}<br>
    Data sent: {% if s.data_sent %}{{ s.data_sent | join: ', ' }}{% else %}—{% endif %}<br>
    Endpoint: {{ s.endpoint | default: '—' }}<br>
    Retention: {{ s.retention | default: '—' }}<br>
    Opt-out: {{ s.opt_out | default: '—' }}<br>
    Docs: {% if s.docs %}<a href="{{ s.docs }}" rel="noopener" target="_blank">Provider policy/docs</a>{% else %}—{% endif %}
  </li>
{% endfor %}
</ul>
{% else %}
No public details available at this time. This section will be updated as implementations are finalized.
{% endif %}

## 7. Analytics and Crash Reporting

We may use platform diagnostics or third‑party tools for analysis and troubleshooting. Availability and data sent vary by version. Please also check in‑app settings and release notes.

## 8. Your Rights

Where applicable, you may have rights to access, correct/update, delete, or withdraw consent for your data. Please contact us through the in‑app support channel to exercise these rights.

## 9. Security

We apply reasonable technical and organizational measures to protect information, but cannot guarantee absolute security for data transmitted over the Internet.

## 10. Age Rating

The App has an App Store age rating of 16+. Users under 16 are not permitted to use the App. If you are 16–17, please use the App with parental consent.

Note: Tumblr platform age requirements also apply (EU: 16+, others: 13+).

## 11. Changes to This Policy

We may update this Policy as laws or services change. We will notify important changes on this page.

## 12. Contact

For privacy inquiries, please use the in‑app Help/Support channel. Using the in‑app flow ensures relevant app and device information is included, enabling faster support.

## 13. Tumblr User-Generated Content

The App displays user‑generated content hosted on Tumblr. The content you see depends on your Tumblr account settings (e.g., Safe Mode).

Content moderation and filtering are managed by Tumblr. The App displays content as returned by the Tumblr API.

## 14. Developer Info

- Developer: Keisuke Isono
- How to contact: via in‑app Help/Support

## 15. Data Deletion

- On‑device data: uninstalling the App removes all on‑device data
- Tumblr data: posts/likes tied to your Tumblr account must be deleted on Tumblr
- OAuth tokens: use the App’s “Log out” to delete tokens

---

Note: This is the privacy policy for Tumblium. It will be updated as necessary when features or external services change.
