# Xsilent Troubleshooting

This page covers common public support steps for Xsilent, without exposing internal implementation details.

## I cannot unlock Xsilent

- Confirm that you are entering the intended PIN.
- If biometric access is enabled, confirm that Android still recognizes the configured biometric method.
- Restart the app and try again.
- If the issue continues, contact support before taking destructive actions.

**Important:** Do not uninstall Xsilent, clear its app data or reset your device as a troubleshooting step without first ensuring that you have a usable backup and the information needed to restore it.

Support: support@tsidevstudio.com

## Biometric access is unavailable

Check that:

- A supported biometric method is configured in Android.
- Biometric authentication is enabled for Xsilent where available.
- The device has not temporarily disabled biometric access after a security change or restart.

Hidden fingerprint unlock is a Lifetime feature and requires a compatible device.

## I cannot see my photos in Xsilent's import screen

Starting with Xsilent 2.4.7, photos and videos are selected through Android's system Photo Picker rather than an in-app device gallery.

To import:

1. Unlock Xsilent.
2. Open the intended vault.
3. Tap **+ Add**.
4. Choose the photos or videos in Android's system picker.
5. Follow the on-screen import instructions.

Xsilent does not request broad access to your entire photo gallery.

If a photo or video is missing from the picker, check whether it is available to Android's system picker or the source application.

You can also share supported media directly from your Gallery to Xsilent using Android's Share function.

## How many files can I import at once?

The maximum number of files per import batch depends on your plan:

- **Free:** up to 10 files per batch.
- **Lifetime:** up to 20 files per batch.

The applicable limit is the same in the main vault and the decoy vault.

Some supported media types may have additional per-batch restrictions.

If you select more files than your plan allows on a device whose system picker does not enforce the limit directly, Xsilent rejects that selection without importing those files.

Try again with fewer files.

## I have used my 30 free imports

Xsilent includes:

- 30 free imports in the main vault.
- 30 independent free imports in the decoy vault.

There is no time limit.

After using your free import allowance:

- Your existing files remain accessible.
- You can continue viewing, sharing, exporting and deleting them.
- You can create encrypted backups.
- You can restore your files according to the backup recovery rules.
- New imports require Lifetime.

Deleting files does not restore previously consumed free imports.

Lifetime removes the total import allowance restriction through a one-time Google Play purchase.

## My original photos are still visible in Gallery

This is expected.

Xsilent 2.4.7 imports photos, videos and supported documents as encrypted copies.

**Importing a file does not automatically remove its original from your Gallery or original location.**

To remove an original from the Gallery:

1. Confirm that the encrypted copy was successfully imported into Xsilent.
2. Open the original file in your Gallery or file manager.
3. Delete it there if you no longer want it visible outside Xsilent.

Check your device's Gallery Trash or Recently Deleted folder if you also want to remove recoverable Gallery copies.

**Do not delete an original before confirming that its encrypted copy is accessible in Xsilent.**

## An imported file is missing from my vault

Check that:

- You are viewing the vault into which you imported the file.
- The import completed successfully.
- The file type is supported.
- The import was not cancelled or interrupted.
- Sufficient local storage was available.

If the import failed, the original should still be available at its source location.

Do not delete the original unless you have confirmed a successful import.

## Screenshot protection behaves differently on my device

Screenshot and screen-recording restrictions depend partly on Android and device-specific behavior.

Some system interfaces or external capture methods may behave differently from in-app capture restrictions.

## A PDF or file does not open as expected

Confirm that:

- The file is supported.
- The file is not corrupted.
- The file was fully imported.
- Sufficient local storage is available.

PDFs and supported documents are selected through Android's system document picker.

If the issue persists, contact support with the file type and Android/device information.

Do not send sensitive private files to support unless you have deliberately chosen to share them.

## Backup or restore issue

Encrypted backup and restore are included in Free.

Before retrying:

- Confirm that the backup file is available and complete.
- Confirm that you are using the intended backup.
- Avoid modifying the backup file.
- Keep the original backup copy until recovery is complete.

### Restoring into an empty vault

A full recovery into an empty vault is not blocked by the Free import allowance.

This allows users to recover their existing supported backup content, even if the backup contains more than 30 files.

Restored files count toward the free import allowance. When it is exhausted, additional new imports require Lifetime.

### Restoring into a vault that already contains files

For Free users, newly restored files are subject to the remaining import allowance.

If the backup contains more files than the remaining allowance permits, the restoration may be partial.

The original backup is not deleted or modified by a partial restoration.

Lifetime removes the total import allowance restriction.

For additional guidance, see [Encrypted Backup](encrypted-backup.md).

## Security issues

Do not report suspected vulnerabilities publicly.

See:

[Security Policy](../SECURITY.md)

## Contact support

For additional help:

support@tsidevstudio.com

Security & Help:

https://tsidevstudio.com/apps/xsilent/security-help

## Privacy note

This troubleshooting guide intentionally avoids internal source-code, cryptographic, storage-layout and authentication details.
