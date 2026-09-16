# Changelog

## 3.2

- Made the initial Flash step strictly read-only for all supported products and
  both G4 and F4 firmware families.
- Deferred writing the zero calibration image until the workflow advances into
  the selected calibration stage.
- Ensured that manual mode performs no Flash write before the user selects
  **Next Step**.
- Continued directly into calibration without an initial write when valid
  previous Flash data is selected.

## 3.1

- Initial public Windows x64 release of BEAR Calibration Tool.
- Added the graphical ADC, Electric Offset, External Encoder, and Torque
  Compensation calibration workflow.
- Added G4/F4 product-profile support, bilingual UI, concise reports, and the
  Windows installer.
