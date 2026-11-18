# onyxia-licenses

Public file server for **Onyxia EA** license tokens (this repository holds no secrets).

- `licenses/<hash>.lic` — one signed license token per device. `<hash>` = first 12 bytes of SHA-256(Device ID), hex.
- Every token is signed with RSA-2048 by the developer's private key. The EA verifies the signature, the device and the
  expiry itself, so a file that is edited or copied to another device is rejected.
- Files are written automatically by `tools/onyxia-license-tool` (Telegram bot / CLI) in the private source repository.
  **Do not edit them by hand.**

## For customers
For automatic license renewals add `https://raw.githubusercontent.com` in MetaTrader 5:
**Tools > Options > Expert Advisors > Allow WebRequest for listed URL**.
Without it everything still works, but you must copy the new `Onyxia_Pro.lic` into `MQL5\Files` yourself.

Support / licensing: https://t.me/onyxia_ea
