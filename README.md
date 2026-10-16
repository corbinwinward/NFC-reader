# NFC Reader

A single-page website (`index.html`) that reads an NFC tag in the browser and shows the parsed NDEF records plus raw hex data.

**Requirements:** Chrome on Android, NFC enabled, page served over HTTPS (Web NFC does not work on iOS or desktop).

Host it with GitHub Pages (Settings → Pages → deploy from branch, root), or any static HTTPS host, then open the URL on your phone.

## iPhone

iOS browsers can't use Web NFC, and Shortcuts has no action that returns tag data. Use an Android phone, or an iOS NFC app. The page can still display data passed as `?id=`, `payload=`, `hex=` or `b64=`.
