# Public release checklist

- [x] Version 3.5 Windows x64 installer has passed native/core, workflow, GUI,
      legal-document, and customer-package gates during packaging.
- [ ] The 3.5 Release page uses the verified installer and publishes its exact
      SHA-256 value.
- [ ] On representative supported products, confirm Torque Compensation's
      bidirectional acquisition and Friction Compensation's fit, warning,
      readback, safe stop, and default-off behavior with the released installer.
- [ ] Confirm the default report/plot output and optional `runtime.dat`
      `output=1` CSV export in their expected results folders.
- [x] EULA, safety, privacy, security, and translations are the approved release
      versions.
- [ ] Automated tests and the hardware regression test passed for the exact
      release commit and supported product/firmware profiles.
- [ ] A clean Windows machine completed install, launch, calibration-simulator or
      approved hardware smoke test, upgrade, and uninstall validation.
- [ ] For both G4 and F4 hardware, the initial Flash step performs no write. With
      previous Flash disabled in manual mode, the zero image is written only
      after **Next Step** and before the selected calibration stage begins.
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
