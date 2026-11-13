# ClipLift Privacy Policy

**Your saved text. Your choice.**

**Effective date:** November 13, 2026  
**Applies to:** ClipLift version 1.0.0  
**Publisher:** Yuvaraja, under **Ynygma LTD**

ClipLift is a Chrome extension that lets you save selected text in two local clipboard slots and optionally display currency-conversion tags on supported websites. This policy explains what information ClipLift accesses, why it needs that information, where it is stored, and the choices available to you.

## 1. Information ClipLift accesses and why

- **Text you choose to save.** When you explicitly save selected text to a slot, ClipLift processes and stores that text so you can retrieve or copy it later. Text you select may contain personal, confidential, or sensitive information. ClipLift does not automatically read your device's clipboard or save text from password fields.
- **Visible website text for optional currency conversion.** When currency conversion is enabled, ClipLift examines visible text on supported websites locally to identify prices and currencies and display reference-rate tags. Website text is not sent to Ynygma LTD or to the exchange-rate provider.
- **Site information needed for features.** ClipLift uses tab URLs or page origins temporarily to direct an explicit clipboard action to the correct tab and apply site-specific conversion preferences. It stores hostnames you choose to exclude from conversion. It does not keep a history of the pages you visit.
- **Your settings and rate data.** ClipLift stores currency preferences, excluded hostnames, timestamps for saved slots, and cached exchange-rate information to provide its features.

ClipLift uses this information only to perform the functions described above.

## 2. Local storage, security, and retention

Saved text, slot timestamps, preferences, excluded hostnames, and exchange-rate caches are stored locally in your Chrome profile. ClipLift does not provide an account or upload these records to a server operated by Yuvaraja or Ynygma LTD.

Saved snippets are encrypted using **AES-256-GCM** before being stored. The non-extractable encryption key is held in the extension's IndexedDB storage within the same Chrome profile. Preferences and cached rates are stored in ordinary Chrome extension storage and are not covered by the snippet-encryption claim.

Saved snippets remain until you replace or clear them, clear the extension's local data, or uninstall ClipLift. Cached rates and preferences remain until replaced or the relevant local data is cleared. A successful rate snapshot is normally reused for up to **12 hours**; if a fresh request fails, a snapshot fetched within the preceding **seven days** may be used and identified as cached.

Encryption helps protect locally stored snippets, but it does not eliminate all risks. Someone with access to your device, Chrome profile, or backups may be able to obtain locally stored information. Clearing a slot does not erase text you have already pasted elsewhere, copies held by other applications, or copies that may remain in device backups.

If you copy saved text to your device's clipboard, the operating system and other applications with clipboard access may be able to read it. That clipboard content is outside ClipLift's local slot storage.

## 3. Exchange-rate service and network information

**Only when currency conversion is enabled**, ClipLift makes HTTPS requests to [Frankfurter](https://frankfurter.dev/) at [api.frankfurter.dev](https://api.frankfurter.dev) to obtain reference exchange rates. Requests include the currency codes necessary to return rates. They do **not** include saved snippets, website text, visited-page URLs, or website cookies.

The connection passes through infrastructure used by the exchange-rate service, which may technically handle network information such as an IP address and request time. According to [Frankfurter's published FAQ](https://frankfurter.dev/), its public API does not collect or log personal data, IP addresses, or request URLs and uses Cloudflare for caching and protection. Frankfurter is an independent third-party service; its practices may change.

Currency tags show reference conversions, not guaranteed live transaction prices. Where available, you can hover over a tag to see the date of the exchange-rate data.

## 4. Your controls

You can clear either saved-text slot, replace its contents, disable currency conversion, or exclude an individual website hostname from conversion. Chrome's extension controls also allow you to restrict site access, disable ClipLift, clear its local data, or uninstall it. Restricting access may prevent some ClipLift features from working.

ClipLift's page content scripts receive only the conversion settings and rate information needed for the current website, including whether that hostname is excluded. Saved snippets are handled by ClipLift's background service worker and extension pages, not passed to website content scripts.

Because saved snippets are not stored on a ClipLift server, Yuvaraja and Ynygma LTD cannot retrieve, remotely change, or remotely delete the local snippets in your Chrome profile. For local deletion, use the controls described above.

## 5. Sharing, advertising, and analytics

ClipLift does not send saved snippets or website content to Yuvaraja, Ynygma LTD, advertisers, or analytics providers. Version 1.0.0 has no advertising SDK, analytics SDK, payment processing, or ClipLift account system. ClipLift does not sell user data or transfer it for advertising, creditworthiness assessment, or lending.

The external service used for currency conversion is **Frankfurter**, as explained in Section 3. Its infrastructure can handle the technical information necessary to complete an exchange-rate request. No selected text or website content is intentionally shared with that service.

**Google Limited Use statement:** The use of information received from Google APIs will adhere to the [Chrome Web Store User Data Policy](https://developer.chrome.com/docs/webstore/program-policies/limited-use), including the Limited Use requirements.

## 6. Privacy questions, requests, and changes

For privacy questions, concerns, or requests relating to ClipLift, contact **Yuvaraja on behalf of Ynygma LTD** using the support contact published on ClipLift's Chrome Web Store listing. Requests will be reviewed in accordance with applicable law. Where applicable, you may have rights to request information, access, correction, or deletion of personal data. The local-only nature of saved snippets limits what we can access or change on your behalf.

If ClipLift's data-handling practices materially change, this policy will be updated, including its effective date. Where required, additional notice or consent will be provided before a new practice begins.

---

*ClipLift · Save text. Stay organized.*
