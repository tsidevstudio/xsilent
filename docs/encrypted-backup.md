# Xsilent Encrypted Backup

Xsilent supports encrypted backup and restore for users who want a portable recovery option for supported vault content.

**Encrypted backup and restore are available in both Free and Lifetime.**

This document describes only public, user-facing behavior.

## Why use a backup

A backup can help reduce the risk of losing private content because of device loss, device replacement or local data failure.

A backup should be treated as sensitive data even when encrypted.

## Backup availability

Encrypted backup is included in the free version of Xsilent.

- No Lifetime purchase is required to create an encrypted backup.
- You can back up your existing vault files even after using all 30 free imports.
- You choose where the encrypted backup is saved.
- Lifetime users have access to the same backup and restore functionality.

## Restoring your files

Xsilent supports restoring encrypted backups.

### Full recovery into an empty vault

If you are recovering your files into an empty vault, Xsilent allows you to restore your valid backup content even if it contains more than 30 files.

The free import limit does not prevent you from recovering your existing files.

Restored files count toward the free import allowance. If the allowance is exhausted, new imports require Lifetime.

Existing restored files remain accessible.

### Restoring into a vault that already contains files

When restoring a backup into a non-empty vault, Xsilent applies the remaining free import allowance to newly restored files.

- Free users can restore additional files up to their remaining allowance.
- If the allowance is reached, the restore may be partial.
- Lifetime users do not have the total import allowance restriction.

The source backup is not deleted or modified by a partial restore.

## Your files remain accessible

Using all 30 free imports does not lock your existing files.

You can continue to view, share, export, delete, back up and restore your files according to the applicable recovery rules.

Deleting files does not restore previously consumed free imports.

## Good backup practices

- Store backups only in locations you trust.
- Keep more than one copy when the content is important.
- Avoid sharing backup files with other people.
- Protect any recovery information associated with your backup.
- Periodically confirm that your backup workflow still works as expected.
- Remove obsolete backup copies when they are no longer needed.
- Check that important files are accessible after a restore.

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
