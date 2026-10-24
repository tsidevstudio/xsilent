# Xsilent Encrypted Backup

Xsilent supports encrypted backup for users who want a portable recovery option for supported vault content.

This document intentionally describes only public, user-facing behavior.

## Why use a backup

A backup can help reduce the risk of losing private content because of device loss, device replacement or local data failure.

A backup should be treated as sensitive data even when encrypted.

## Good backup practices

- Store backups only in locations you trust.
- Keep more than one copy when the content is important.
- Avoid sharing backup files with other people.
- Protect any recovery information associated with your backup.
- Periodically confirm that your backup workflow still works as expected.
- Remove obsolete backup copies when they are no longer needed.

## Local control

Xsilent does not require users to place vault backups in a specific cloud service.

Users remain responsible for choosing where backup files are stored.

## Security boundary

For security and intellectual-property reasons, TSI Dev Studio does not publish the internal backup specification.

This repository does not document:

- Backup container structure.
- Internal file layout.
- Key derivation parameters.
- Encryption implementation details.
- Nonce or key-management behavior.
- Internal restore-validation logic.

## Help

https://tsidevstudio.com/apps/xsilent/security-help

support@tsidevstudio.com
