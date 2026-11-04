# Xsilent Privacy Features

Xsilent is a privacy-focused Android vault for photos, videos, PDFs and private files.

This document describes user-visible privacy features at a high level. It does not describe the application's internal architecture, source code, cryptographic implementation, key-management logic, storage layout or security-sensitive decision flows.

## Local-first design

Xsilent is designed around local control of private content.

Core vault usage does not require:

- An Xsilent account.
- Advertising.
- Mandatory cloud storage.
- Broad access to your photo gallery.

Files stored in the vault remain under the user's local control.

## Android Photo Picker and file privacy

Xsilent uses Android's system Photo Picker for selecting photos and videos.

PDFs and other supported documents are selected through Android's system document picker.

Xsilent does not require broad access to your entire photo gallery. It accesses only the files you explicitly choose or share.

### Encrypted copies

When you import a file into Xsilent, the app saves an encrypted copy inside the vault.

**The original file remains in your Gallery or at its original location.**

Xsilent does not automatically delete originals during import.

If you want to remove the original from your Gallery, first confirm that the encrypted copy is available inside Xsilent, then delete the original manually.

## PIN protection

Xsilent uses PIN-based access controls to protect entry to the vault.

The main vault and the decoy vault provide separate user-facing storage experiences.

This public documentation intentionally does not describe authentication internals or decision logic.

## Fake PIN and decoy vault

Xsilent includes a **Fake PIN** feature that opens a separate decoy vault experience.

The Fake PIN and decoy vault are included in the Free version.

Internal separation, verification, storage and access-control mechanisms are not documented publicly.

## Biometric access

Where supported by the device and Android version, biometric authentication can be used as an additional convenience layer for accessing Xsilent.

Lifetime includes a hidden fingerprint unlock option.

Feature availability may depend on the device and its supported biometric capabilities.

## Quick Lock and automatic locking

Xsilent includes locking controls intended to reduce the time private content remains visible when the user is no longer actively using the vault.

These include:

- Quick Lock.
- Automatic locking behavior.
- Privacy-focused background handling.

Exact internal trigger logic is intentionally not documented publicly.

## Screenshot and screen-recording protection

Where supported, Xsilent can restrict screenshots and screen recording in sensitive parts of the app.

Behavior may vary depending on Android version, device implementation and system limitations.

## Private PDF viewing

Xsilent can display supported PDFs within the privacy-focused vault experience.

Private PDF viewing is included in Free.

## Clean Share

Clean Share provides privacy-oriented sharing tools intended to help users prepare content before sharing it outside Xsilent.

Supported privacy operations include:

- Blurring faces.
- Removing metadata.
- Additional privacy adjustments where available.

Clean Share is included in Lifetime.

## Encrypted Trash

Xsilent includes an encrypted Trash feature for supported deleted vault content.

Trash behavior is designed to provide a recovery window while keeping deleted content within the protected Xsilent environment until permanent removal.

Encrypted Trash is included in Free.

## Encrypted backup

Xsilent supports encrypted backup and restore for users who want a portable recovery option.

Encrypted backup and restore are included in Free.

A full recovery into an empty vault is not blocked by the free import allowance. Restoring into a non-empty vault follows the remaining free import allowance.

For further public guidance, see [Encrypted Backup](encrypted-backup.md).

For security and intellectual-property reasons, this repository does not publish:

- Backup container structure.
- Key derivation details.
- Encryption parameters.
- Internal metadata layout.
- Authentication or restoration internals.

## Free and Lifetime privacy features

Xsilent can be installed and used for free, without a time-limited trial.

### Free

- 30 free imports in the main vault.
- 30 independent free imports in the decoy vault.
- Up to 10 files per import batch.
- Fake PIN and decoy vault.
- Encrypted backup and restore.
- Encrypted Trash.
- Private PDF viewing.
- PIN protection, Quick Lock and automatic locking.
- Security Center.

Using all free imports does not lock existing files. Users can continue accessing, sharing, exporting, deleting and backing up their files.

Deleting files does not restore consumed free imports.

### Lifetime

Lifetime is a one-time purchase through Google Play that provides:

- Unlimited total imports.
- Up to 20 files per import batch.
- Hidden fingerprint unlock.
- Clean Share.
- Everything included in Free.

No subscription or recurring fees are required.

The exact local price is displayed by Google Play before purchase.

## Privacy model

Xsilent is designed to reduce unnecessary external dependence during normal private-vault use.

- No required Xsilent account.
- No advertising.
- No mandatory cloud storage.
- No broad photo-gallery access permission.
- Local-first operation.
- User-controlled encrypted backup.

## Official resources

- Xsilent: https://tsidevstudio.com/apps/xsilent
- Privacy Policy: https://tsidevstudio.com/privacy/xsilent
- Security & Help: https://tsidevstudio.com/apps/xsilent/security-help
- Google Play: https://play.google.com/store/apps/details?id=com.xsilent.app
