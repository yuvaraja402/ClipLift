# ClipLift Privacy Policy

**Your browser. Your saved text.**

Privacy policy for **ClipLift 1.0.0**  
**Effective date:** November 13, 2026

## What ClipLift handles

ClipLift is published by Yuvaraja. It provides two text clipboard slots and optional currency tags on supported websites. It handles the text you explicitly select for saving, visible price text when conversion is enabled, currency preferences, and hostnames you choose to exclude from conversion.

Clipboard snippets may contain personal information that you choose to copy. ClipLift does not automatically read your system clipboard or save text from password fields.

## What stays in Chrome

Saved snippets, the time each slot was saved, preferences, excluded hostnames and cached exchange rates are stored locally in this Chrome profile. Saved snippets remain until you replace or clear them, clear the extension's storage, or uninstall the extension. ClipLift does not sync these records through a ClipLift account or a server.

Visible website text is examined locally to identify price amounts and currencies. It is not uploaded. Tab URLs and page origins are used in memory to route explicit clipboard commands and apply site preferences. ClipLift does not keep a record of your browsing history.

Saved snippets are encrypted with AES-256-GCM before they are persisted. The non-extractable encryption key is kept in the extension's IndexedDB storage in this browser profile. Settings and rate caches remain in ordinary Chrome extension storage. Device access and browser-profile backups can affect the privacy and retention of locally stored information.

## Exchange-rate requests

When you turn currency conversion on, ClipLift requests reference-rate data from Frankfurter at [api.frankfurter.dev](https://api.frankfurter.dev) over HTTPS. The request includes your chosen target currency code. It excludes page URLs, page text, saved snippets and cookies. The provider receives ordinary network information, including your IP address and the time of the request.

A successful snapshot is cached for 12 hours. If a new request fails, a snapshot fetched within the previous seven days can be used and is marked as cached. Per-currency rate dates are available by hovering over the tags. Frankfurter operates its own service independently of ClipLift.

## Your controls

Use each slot's clear button to delete its saved text. Turn currency conversion off to stop automatic price conversion, or use the website checkbox to hide tags on a particular hostname. Chrome's extension settings also let you restrict website access, disable ClipLift or uninstall it. Restricting website access can limit clipboard actions and currency tags.

Clipboard content is available only to ClipLift's service worker and its extension pages. Page content scripts receive the currency configuration and conversion data they need, together with only the current site's exclusion setting.

## Sharing and analytics

ClipLift does not send saved snippets or website content to its publisher, analytics services or advertisers. It has no advertising, analytics SDK, payment processing or account system in this release. Data is used to provide the features described here. User data is not sold or transferred for advertising, creditworthiness or lending purposes.

ClipLift's use of information received from Google APIs follows the Chrome Web Store User Data Policy, including its Limited Use requirements.

## Questions and future changes

Contact the publisher through the Support contact on ClipLift's Chrome Web Store listing for privacy questions. Material changes to how ClipLift handles data will be reflected in an updated policy and effective date.

---

*ClipLift / Copy more. Browse smarter.*
