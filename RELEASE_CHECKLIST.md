# Public release checklist

- [x] EULA, safety, privacy, security, and translations are the approved release
      versions.
- [ ] Automated tests and the hardware regression test passed for the exact
      release commit and supported product/firmware profiles.
- [ ] A clean Windows machine completed install, launch, calibration-simulator or
      approved hardware smoke test, upgrade, and uninstall validation.
- [ ] The installer presents the correct EULA and separately offers Start Menu
      and desktop shortcuts named `BEAR Calibration`.
- [ ] The Simplified Chinese installer page renders the complete Chinese EULA
      correctly, without mojibake or missing glyphs.
- [ ] Uninstall detects a running application, asks before requesting a normal
      close, and removes no files until the process has exited.
- [ ] Every official release channel contains only the installer, SHA-256 value,
      release notes, and any approved public documentation. Do not upload the
      portable staging ZIP or source package.
- [ ] The README safety warning matches the EULA, installed safety notice, quick
      start, and in-application pre-start confirmation.
- [ ] A release owner confirms this checklist before publication.
