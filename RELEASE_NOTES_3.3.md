# BEAR Calibration Tool v3.3 (Windows x64)

Download `BEAR_Calibration_Tool_Setup_Windows_x64_v3.3.exe` from this Release.
The installer SHA-256 is:

`D3A08184806704AA1627E523AEC6551F2DB723D61727D8DC9F0F33524ACC017B`

## What's new

- **Friction Compensation calibration:** measures forward and reverse motion at
  0.1, 0.3, 0.5, 1, 2, 3, and 5 rad/s, fits each actuator's friction parameters,
  and verifies them before updating calibration Flash. Friction compensation
  remains off after calibration for separate on-device evaluation. This stage
  requires compatible BEAR firmware; insufficient supply voltage or an
  unattainable required speed stops the stage without writing its result.
- **Torque Compensation calibration:** aligns bidirectional measurements to
  actual rotor position and removes residual current mean before creating the
  compensation table.
- **Acquisition and diagnostics:** improves Debug 3 telemetry synchronization,
  friction progress and remaining-time updates, and reporting of periodic
  high-speed friction ripple. A qualified ripple produces a warning while the
  baseline fit is retained.
- **Optional CSV output:** the default remains a concise JSON report and
  summary plots. Authorized engineering personnel can set the top-level
  `output` value in `runtime.dat` to `1` and restart the application to save
  detailed CSV files in each calibration session's results folder.

## Before use

BEAR actuators are calibrated before shipment and normally do not need this
utility. For recalibration, disconnect every external load and mechanism,
secure the actuator body, clear its full motion area, and keep an independent
emergency-stop or power-disconnect method within reach. The actuator rotates
during calibration. Use a compatible product profile and firmware, and follow
the EULA and safety notices in the installer.

Verify the downloaded file in PowerShell with:

```powershell
Get-FileHash .\BEAR_Calibration_Tool_Setup_Windows_x64_v3.3.exe -Algorithm SHA256
```

---

# BEAR Calibration Tool v3.3（Windows x64）

请从本 Release 下载 `BEAR_Calibration_Tool_Setup_Windows_x64_v3.3.exe`。
安装包的 SHA-256 为：

`D3A08184806704AA1627E523AEC6551F2DB723D61727D8DC9F0F33524ACC017B`

## 主要更新

- **摩擦补偿校准：**在 0.1、0.3、0.5、1、2、3、5 rad/s 下采集正反转数据，
  逐台拟合摩擦参数，验证后写入校准 Flash。校准结束后摩擦补偿保持关闭，供用户
  在设备上单独开启并验证。此步骤需要兼容的 BEAR 固件；供电电压不足或达不到
  要求的测试速度时，该步骤会停止且不写入结果。
- **扭矩补偿校准：**根据实际转子位置对齐双向测量数据，生成补偿表前去除残余
  电流均值。
- **采集与诊断：**改进 Debug 3 遥测同步、摩擦校准进度与剩余时间显示，以及高速
  周期性摩擦波动的提示。符合条件的波动会给出警告，同时保留基准拟合结果。
- **可选 CSV 导出：**默认仍保存精简 JSON 报告和摘要图。获授权的工程人员可将
  `runtime.dat` 顶层的 `output` 设为 `1`，重启程序后在每次校准的结果文件夹中
  保存详细 CSV。

## 使用前

BEAR 驱动器出厂前已完成校准，通常无需使用本工具。重新校准时，必须断开全部
外部负载和机构，固定驱动器本体，清空完整运动区域，并准备独立的急停或断电
手段。驱动器会在校准期间转动。请使用兼容的产品配置与固件，并遵守安装程序中
的 EULA 和安全说明。

可在 PowerShell 中使用以下命令核对下载文件：

```powershell
Get-FileHash .\BEAR_Calibration_Tool_Setup_Windows_x64_v3.3.exe -Algorithm SHA256
```
