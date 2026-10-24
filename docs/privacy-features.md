# Xsilent Privacy Features

Xsilent is a privacy-focused Android vault for photos, videos, PDFs and private files.

This document describes user-visible privacy features at a high level. It does not describe the application's internal architecture, source code, cryptographic implementation, key-management logic, storage layout or security-sensitive decision flows.

## Local-first design

Xsilent is designed around local control.

Core vault usage does not require:

- An Xsilent account.
- Advertising.
- Mandatory cloud storage.

## PIN protection

Xsilent uses PIN-based access controls to protect entry to the vault.

Users may also use supported biometric authentication for convenient access.

This public documentation intentionally does not describe authentication internals or decision logic.

## Decoy PIN

Xsilent includes a Decoy PIN feature designed to provide an alternative vault experience when a different PIN is entered.

The public description is intentionally limited to user-visible behavior.

Internal separation, verification, storage and access-control mechanisms are not documented publicly.

## Biometric access

Where supported by the device and Android version, biometric authentication can be used as an additional convenience layer for accessing Xsilent.

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

## Clean Share

Clean Share provides privacy-oriented sharing tools intended to help users prepare content before sharing it outside Xsilent.

Depending on the supported content and workflow, privacy tools may include operations such as metadata removal or visual privacy adjustments.

## Encrypted Trash

Xsilent includes an encrypted Trash feature for supported deleted vault content.

Trash behavior is designed to provide a recovery window while keeping deleted content within the protected Xsilent environment until permanent removal.

## Encrypted backup

Xsilent supports encrypted backup for users who want a portable recovery option.

For security and intellectual-property reasons, this repository does not publish:

- Backup container structure.
- Key derivation details.
- Encryption parameters.
- Internal metadata layout.
- Authentication or restoration internals.

For public user guidance:

https://tsidevstudio.com/apps/xsilent/security-help

## Official resources

- Xsilent: https://tsidevstudio.com/apps/xsilent
- Privacy Policy: https://tsidevstudio.com/privacy/xsilent
- Security & Help: https://tsidevstudio.com/apps/xsilent/security-help
- Google Play: https://play.google.com/store/apps/details?id=com.xsilent.app
