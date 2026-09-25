# kongyiflyapp (encrypted source mirror)

This repository stores an **AES-256 encrypted mirror** of the KongYiFly App
source code. Every file under `enc/` is AES-256-CBC + PBKDF2 encrypted and
base64 encoded — without the password it is unreadable.

The restore script is **not** included in this repository; it is kept
offline by the author together with the password. Wrong / lost password =
the backup cannot be restored.

## Layout

```
enc/lib/...          encrypted source files (one .b64 per source file)
enc/android/...      encrypted android project files
enc/pubspec.*.b64    encrypted project manifests
```

© 2026 kyfly
