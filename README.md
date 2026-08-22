# Dosiary

A small, private desktop diary for recording medication doses and the exact
time they were taken.

Dosiary keeps its data on the device. It has no account, backend, analytics, or
network-based health features. It is an organizational record only and does not
provide medication reminders, dosage recommendations, or medical advice.

**[Download the latest version](https://github.com/Haembina/dosiary-releases/releases/latest)**

This repository exists only to host those downloads. The source is kept
privately by [Haembina](https://haembina.com).

## Installing on Windows

Every build is 64-bit. There is no 32-bit or ARM64 installer, so a Windows on
ARM device cannot run these.

Two installers are published with every release. Take the first unless you have
a reason not to:

| File | Use it when |
| --- | --- |
| `Dosiary_x.y.z_x64-setup.exe` | Normal install. This is the one in-app updates use. |
| `Dosiary_x.y.z_x64_en-US.msi` | You deploy software through Group Policy or Intune. |

`latest.json` is not a download. It is the file an installed copy reads to
discover new versions.

### "Windows protected your PC"

The installer is not signed with a Windows code-signing certificate, so
SmartScreen shows a blue warning the first time it runs. To continue, choose
**More info**, then **Run anyway**.

That warning reflects the absence of a paid certificate rather than anything
detected in the file. If you would rather be careful, download only from the
releases page linked above.

## What Dosiary does

- Log a dose with one click
- Configure four frequently used dosage amounts
- See the time elapsed since the latest dose
- Browse and edit entries by date
- Flag an entry when the recorded dose is uncertain
- Minimize to the system tray with the latest-dose status

## Updates

From 1.1.0 onward, Dosiary checks this page when it starts and offers any newer
version as a button beside the version number in its footer. Nothing downloads
or installs on its own.

Every update is signed, and the app verifies that signature against a key built
into it before installing anything. A file that is not signed with Dosiary's
own key is refused, so a tampered installer cannot arrive through the updater.

Versions 1.0.2 and earlier have no updater and need to be replaced by hand,
once.

## Privacy

Doses are stored locally by the application and are never transmitted. The only
network request Dosiary makes is the update check against this repository,
which sends nothing about your data.
