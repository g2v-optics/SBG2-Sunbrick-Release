# Sunbrick Desktop App – Releases

This repository hosts the public releases of the **Sunbrick** desktop
application by [G2V Optics](https://g2voptics.com). It contains no source
code: each entry on the [Releases](../../releases) page is a published
version of the app with its installers, release notes and authentication
record.

## Downloading and installing

Open the [latest release](../../releases/latest) and pick the file for your
platform:

| Platform | File | Notes |
|---|---|---|
| Windows 10 / 11 (64-bit) | `Sunbrick-Setup-<version>.exe` | Recommended. Signed installer with automatic updates. |
| Windows, portable | `Sunbrick-<version>-win.zip` | Unzip and run. Does not auto-update. |
| Linux x86_64 | `Sunbrick-<version>.AppImage` or `sunbrick_<version>_amd64.deb` | |
| Linux arm64 | `Sunbrick-<version>-arm64.AppImage` or `sunbrick_<version>_arm64.deb` | |

The AppImage needs to be made executable before it runs
(`chmod +x Sunbrick-<version>.AppImage`).

## Automatic updates

The installed Windows app checks this repository for new versions. Open
**About → Software Update → Check for updates** inside the app to update, or
download the newer installer from the releases page and run it over the
existing installation.

## What is in a release

| File | What it is |
|---|---|
| Installers (see above) | The application for each platform |
| `authentication_<version>.pdf` | G2V's authentication record for the release: the list of changes, the repository and the exact commit the build was made from |
| `latest.yml`, `latest-linux.yml`, `*.blockmap` | Metadata used by the app's updater. Nothing to download by hand |
| `sunbrick-integration-scripts-<version>.zip` | Scripts used by G2V for installation and bench testing. Not needed for normal use |

## Reading the release notes

- Each release lists **every change since the previous version published
  here**, not just since G2V's previous internal build. Several internal
  versions are usually tested between two public releases, and their changes
  are all included in the next public release's notes.
- Changes are grouped into **Features**, **Bug Fixes** and other sections.
  Internal work (test benches, release tooling, documentation, CI) is left
  out.
- Tags such as `[MH60237-1234]` are G2V's internal ticket numbers, and the
  links next to each entry point to G2V's private development repository.
  They are there for traceability and will not open for you.
- Version numbers follow `major.minor.patch`. A patch release fixes bugs; a
  minor release adds features; a major release may change how existing
  features work.

## Reporting a problem

Contact G2V Optics support at [g2voptics.com](https://g2voptics.com), or
reach out to your G2V contact directly. Please include the app version
(shown in **About**) and the steps to reproduce.

## License

Use of the Sunbrick app is subject to G2V's End User License Agreement. See
[LICENSE](LICENSE), or the current version at
<https://g2voptics.com/legal/eula/>.
