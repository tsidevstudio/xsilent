# Xsilent Changelog

This changelog summarizes notable public, user-facing Xsilent changes.

It intentionally does not document internal architecture, private implementation details, security-sensitive logic or source-code changes.

## 2026

### November

#### Xsilent 2.4.7 (23) — Privacy and Import Improvements

**Android Photo Picker**
- Introduced Android's system Photo Picker for selecting photos and videos.
- Removed the need for broad photo-gallery access permissions.
- Continued support for importing PDFs and supported documents through Android's system file picker.
- Photos, videos and supported files are imported as encrypted copies.
- Original files remain in their Gallery or original location and are not automatically deleted.

**Free and Lifetime**
- Introduced 30 free imports in the main vault and 30 independent free imports in the decoy vault.
- Free users can import up to 10 files per batch.
- Lifetime users can import up to 20 files per batch, with unlimited total imports.
- Free imports have no time limit.
- Existing files remain accessible after the free import allowance is used.
- Deleting files does not restore consumed free imports.
- Fake PIN, encrypted backup and restore, encrypted Trash and private PDF viewing remain available in Free.

**Backup and Recovery**
- Improved recovery behavior for encrypted backups.
- Full recovery into an empty vault is not blocked by the free import allowance.
- Restoring additional files into a non-empty vault follows the remaining Free import allowance.
- Existing files remain accessible after the import allowance is exhausted.

**Privacy and Usability**
- Improved navigation when returning from full-screen media viewers.
- Improved privacy when returning to Xsilent from the background.
- Improved import confirmation messages and guidance about original Gallery files.
- Additional stability and reliability improvements.

### October

- Introduced the current Free and Lifetime access model.
- Added and refined public Free vs Lifetime information.
- Expanded Security Center and security-related guidance.
- Expanded encrypted backup support and user guidance.
- Improved private PDF and file handling.
- Added or refined Clean Share privacy tools.
- Added or refined screenshot and screen-recording protection where supported.
- Improved Quick Lock and automatic locking behavior.
- Expanded encrypted Trash behavior and recovery guidance.
- Added broader product documentation and public security/help resources.
- Expanded website localization and public product information.

### Earlier 2026

- Continued improvements to local-first vault usage.
- Improved biometric access and PIN-protected vault workflows.
- Expanded support for private photos, videos, PDFs and files.
- Added Decoy PIN support for an alternative vault experience.
- Continued usability, privacy and reliability improvements.

## Notes

Xsilent is actively maintained.

Not every internal maintenance change is listed here. Security-sensitive implementation changes may be intentionally omitted from public release notes.

Official product information:

https://tsidevstudio.com/apps/xsilent
