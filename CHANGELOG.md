# Changelog

## 3.5

- Improved calibration measurement accuracy and consistency across supported products.
- Enhanced compensation calibration reliability and result handling.
- Fixed known issues and improved diagnostic reporting.

## 3.4

- Improved calibration accuracy and reliability across supported products.
- Improved compensation calibration and corrected known issues.

## 3.3

- Added per-actuator Friction Compensation calibration using paired forward and
  reverse measurements at seven output speeds. The fitted parameters are
  verified before Flash write, and friction compensation remains off afterward.
- Added runtime product settings for the friction voltage check and velocity
  controller. The calibration stops without writing its result when supply
  voltage or attainable speed is insufficient.
- Updated Torque Compensation to align bidirectional measurements by actual
  rotor position and remove residual current mean before table quantization.
- Added an optional detailed CSV export for calibration data through the
  top-level `runtime.dat` `output` setting; the default remains summary output.
- Improved Debug 3 telemetry synchronization, friction acquisition progress,
  and handling of high-speed periodic residuals. Qualified high-speed ripple
  produces a warning while retaining the baseline friction fit.

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
