# Privacy policy

**Last updated:** August 16, 2026
**Contact:** development_support@icloud.com

This document describes how the apps listed below handle information. Each app has its own section. Unless a section says otherwise, we do **not** operate a backend that receives your personal content from that app for our own analytics or resale.

**Feedback:** You may use **[GitHub Discussions](https://github.com/dantonoli/developer-support/discussions)** for some apps. That site is operated by a third party with its own privacy policy.

---
## PlainClip

PlainClip is a macOS menu bar utility that cleans the system pasteboard on your Mac.

### What the app does on your device

- **Clipboard (pasteboard):** The app reads and writes the **general pasteboard** only to apply the cleaning features you enable (for example plain text conversion, optional URL parameter cleanup, quote normalization, and removal of hidden marker characters). Processing happens **locally on your Mac**. We do **not** receive a copy of your clipboard.
- **Settings:** Your preferences are stored with **UserDefaults** on your device (standard macOS app storage).
- **No account:** PlainClip does not require sign-in.
- **No network:** PlainClip has no network entitlement and makes no network connections.

### Copy fingerprint (optional, off by default)

PlainClip includes an optional feature that embeds an invisible marker into text you copy, so you can tell whether a piece of text originated on your Mac. **It is switched off by default**, and turning it on requires confirming a dialog that explains what the marker is.

- **What the marker contains:** a random per-install identifier, the time of the copy to the minute, and an optional short label you type in Preferences.
- **How the identifier is generated:** it is the first four bytes of a randomly generated UUID, created the first time you use the feature and stored in UserDefaults on your Mac. It is **not** derived from any hardware or device identifier — not your serial number, not a hardware UUID, not a network address. It is not used for advertising, attribution, analytics, or tracking, and it is not linked to your identity.
- **Where it goes:** the marker is written only into your own clipboard. PlainClip never transmits it. It leaves your Mac only inside text that **you** paste or share — and in that case anyone who receives that text could detect and read the marker with a Unicode inspector. Treat marked text the way you would treat any other content you share.
- **How to inspect or remove it:** the menu bar provides “Check clipboard fingerprint” and “Remove copy marker”, and “Clean clipboard now” also removes it. Turning the feature off stops any further marking.
- **Automatic marking:** a separate opt-in sub-setting can mark every qualifying copy automatically. It has its own confirmation, and it deliberately skips clipboards marked private by password managers, copies shorter than 32 characters, and clipboards carrying files or images.
- **No log is kept.** PlainClip does not record what you copied, when you copied it, or which text was marked.

### Removing hidden markers (on by default)

PlainClip can strip invisible marker characters that other apps and tools embed in text, such as variation selectors, Unicode tag characters, and direction-control characters. This works on marker **characters** only. Watermarks that are woven into the word choice of AI-generated text use a different technique and cannot be detected or removed by any character-level tool, including PlainClip.

### What we do not do (PlainClip)

- We do **not** sell your personal information.
- We do **not** use in-app analytics, advertising SDKs, or crash reporters that send data to us in the current product (unless you add them later—then update this section).
- We do **not** track you across other companies’ apps or websites for advertising in the App Tracking Transparency sense.
- We do **not** receive, store, or have any way to read the copy fingerprint. It exists only on your Mac and in text you choose to share.

### Children (PlainClip)

PlainClip is not directed at children under 13, and we do not knowingly collect their personal information through the app.

### Privacy questions (PlainClip)

Use the contact email at the top of this document.

---

## Other apps

Additional apps will be listed in this document when they are published.

---

## Changes

We may update this policy when our apps change. The **Last updated** date at the top will change when we do.