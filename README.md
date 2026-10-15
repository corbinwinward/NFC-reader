# NFC Reader

A single-page website (`index.html`) that reads an NFC tag in the browser and shows the parsed NDEF records plus raw hex data.

**Requirements:** Chrome on Android, NFC enabled, page served over HTTPS (Web NFC does not work on iOS or desktop).

Host it with GitHub Pages (Settings → Pages → deploy from branch, root), or any static HTTPS host, then open the URL on your phone.

## iPhone (Shortcuts bridge)

iOS browsers can't use Web NFC. Instead, create a shortcut: **Scan NFC Tag** → **URL Encode** the Payload and Identifier → **Text** `https://YOUR-SITE/?id=<encoded id>&payload=<encoded payload>` → **Open URLs**. The page decodes the query string (`id`, `payload`, optional `hex` / `b64`) and shows parsed and raw views.
