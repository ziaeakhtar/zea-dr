# zea-dr — app content data

Public content bundles for Zia Eakhtar Apps. Each app has a folder holding an
encrypted update bundle that the app fetches (anonymously, over HTTPS) for its
periodic in-app content refresh.

| App | File |
|---|---|
| Sofra (Halal Recipes) | `sofra/updates.bin` |

## About these files
- Each `*.bin` is **AES-256-GCM encrypted** and is decrypted **on-device** by
  the app. There is **no human-readable data** in this repo.
- No personal data, credentials, or encryption keys are stored here.
- The app only ever reads from here; nothing is written back.

To add another app later, create a new folder (e.g. `myapp/updates.bin`).
