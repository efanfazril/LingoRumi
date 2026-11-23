# LingoRumi by efanfazril: Privacy Policy

*Version 1.1.0. No analytics, no accounts, no server of its own.*

## Summary

- **Rumi ↔ Jawi conversion happens on your device.** Nothing is sent anywhere.
- **Malay ↔ English translation is online.** The text is sent to the translation service shown in the window, **only after you allow that service**. Rumi ↔ Jawi never needs this.
- **History (default ON):** texts you translate are saved on this device and **each is deleted automatically 14 days after it was last used**. You can switch it off, delete one item or delete all.
- No tracking, no ads, no selling of data, no browsing history, no reading of web pages.

## What is processed

| Data | Where it goes | When |
|---|---|---|
| Text in the top box | Processed in memory in the window | Always |
| Text needing translation | Sent over HTTPS to **LibreTranslate** (`libretranslate.com` or the server you set) or **MyMemory** (`api.mymemory.translated.net`) | Only after you press Allow for that service |
| Your IP address | Seen by that service, as with any web request | During translation |
| Your MyMemory email / LibreTranslate key, if you add them | Sent to that service with each request; stored locally | Only if you add them |
| Text selected on a page (right-click menu) | Passed to the window through memory-only session storage (expires in 60 s) | Only when you pick the menu item |
| History (original + results, up to 2,000 characters each, max 200 items) | `chrome.storage.local` on this device | Only if "Save translated texts" is on |
| Preferences, window position/size/pin | `chrome.storage.local` | Always |

Services handle text under their own terms: MyMemory <https://mymemory.translated.net/doc/tos.php>, LibreTranslate <https://libretranslate.com/privacy>. Do not translate confidential text with a service you do not trust; the offline Rumi ↔ Jawi modes send nothing.

## Automatic deletion

Each history item has a 14-day life that restarts when you use the same text again. Expired items are removed by an hourly background check and whenever the extension starts. Switching history off stops saving; items already saved still expire on schedule. Settings > History > **Delete history now**, and Settings > Data > **Clear all stored data**, erase everything immediately. Uninstalling removes all stored data.

In-memory translation cache: kept only while the window is open, never written to disk.

## Fallback between services

In Automatic mode LibreTranslate is tried first (only if you added a key or server), then MyMemory. If a service fails, the next is used **only if you have allowed it too**, and the window always shows which service translated.

## Pages and permissions

When you click the toolbar icon, a small script draws the floating window on that tab. It does not read the page. Optional "Show pinned window on every page" asks Chrome for access to all sites purely to draw the window again; it is off by default. See [SECURITY.md](SECURITY.md).

## Children, changes, contact

A general-purpose utility; it does not knowingly collect personal information. Changes to data handling will update this document and the Settings screen. Contact: see [SECURITY.md](SECURITY.md).
