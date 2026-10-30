# BEAR Calibration Tool

BEAR Calibration Tool is the official Windows calibration utility for supported BEAR actuators from Westwood Robotics Corporation. BEAR products are calibrated before shipment and normally do not require this utility. It is provided free of charge for exceptional recovery, service, or recalibration situations.

## Critical safety warning

**Before every calibration, completely remove every external load from the BEAR actuator. Disconnect its output from every robot, linkage, transmission, tool, fixture, and other mechanism. Secure the actuator body and confirm that the output shaft can rotate freely.**

**The BEAR actuator will rotate during calibration. Do not begin until all people, clothing, cables, tools, and property are outside its full possible motion area and the movement cannot create a hazard. Keep an independent emergency-stop or power-disconnect method within reach. Do not rely on the application's Stop button as the only protective measure.**

## Download and installation

Download the installer only from an official Westwood Robotics distribution channel: the [company website](https://www.westwoodrobotics.io/) or the official [GitHub Releases](https://github.com/Westwood-Robotics/BEAR_Calibration_Tool/releases).
See the [official GitHub Releases](https://github.com/Westwood-Robotics/BEAR_Calibration_Tool/releases) for the current Windows x64 installer and checksum.

Before running it, compare the file's SHA-256 value with the value published through the same official channel. Do not run a repackaged or third-party installer.

The installer lets you select the installation directory and separately choose whether to create `BEAR Calibration` shortcuts on the Windows Start Menu and desktop. Read and accept the displayed EULA and safety information before use. If the application is running when uninstall starts, the uninstaller asks before requesting a normal close and does not remove files until the process has exited.

## Calibration data behavior

Version 3.5 improves calibration accuracy, compensation calibration reliability,
and handling of known issues across supported products.

Version 3.3 introduced Friction Compensation after Torque Compensation. It measures
both directions at several steady speeds, fits parameters for the individual
actuator, and verifies the result before writing the existing calibration Flash
fields. Friction compensation remains off after calibration so the operator can
enable and evaluate it separately. Torque Compensation now uses bidirectional
measurements aligned to actual rotor position to reduce friction-related bias.

Beginning with version 3.2, the initial Flash step is strictly read-only for all
supported products and for both G4 and F4 firmware. If **Use Previous Flash Data**
is selected and the existing data is valid, calibration uses it without an
initial write. If a zero calibration image is required, it is prepared in memory
and written only after the workflow advances into the selected calibration stage.
In manual mode, no Flash write occurs before **Next Step** is selected.

## License, warranty, and responsibility

The Software is proprietary and closed source. It is licensed free of charge for personal and commercial use with supported BEAR products, subject to the EULA supplied with the release. The license does not grant rights to redistribute, resell, sublicense, host, reverse engineer, or modify the Software except where applicable law expressly permits otherwise.

The installed runtime product configuration can be updated by authorized engineering personnel. Values not supplied or expressly approved by Westwood Robotics are user modifications and are loaded at the user's own risk, subject to the EULA and applicable law.

Use of the official, unmodified Software according to its instructions does not, by itself, void an otherwise applicable BEAR hardware warranty. Subject to the warranty terms and applicable law, damage caused by improper operation, calibration while loaded, failure to follow instructions, unauthorized parameter changes, or modification of the Software is not covered by warranty.

To the maximum extent permitted by applicable law, the user is responsible for bodily injury, property damage, equipment damage, and other loss caused by the user's operation, acts, omissions, modifications, or misuse. Westwood Robotics Corporation does not accept liability for such user-caused loss. The controlling EULA preserves any liability and consumer rights that applicable law does not permit the parties to exclude or limit.

Official publication and marketing of this release are limited to the United States and China. Technical availability through a globally accessible download channel does not represent active marketing, local support, legality, or suitability in every jurisdiction.

By default, each calibration session saves one concise JSON report and, where
applicable, summary plots. The report contains version, product, timestamps,
step outcomes, old/new final summary values, quality metrics, and error codes.
Raw and processed samples are not exported by default. Authorized engineering
personnel can set the top-level `output` value in the installed `runtime.dat` to
`1` and restart the application to save detailed CSV data in that session's
results folder. Treat those files as device diagnostic data and share them only
when needed for support.

## Contact

Questions and security reports: info@westwoodrobotics.io  
Website: https://www.westwoodrobotics.io/

---

# BEAR Calibration Tool（中文）

BEAR Calibration Tool 是 Westwood Robotics Corporation 面向受支持 BEAR 驱动器提供的官方 Windows 校准工具。BEAR 产品出厂前已经完成校准，正常情况下无需使用本工具。本工具免费提供，仅用于意外恢复、维修或重新校准。

## 重要安全警告

**每次校准前，必须完全拆除 BEAR 驱动器上的所有外部负载，并将输出端与所有机器人、连杆、传动装置、工具、夹具和其他机构断开。固定驱动器本体，并确认输出轴可以自由转动。**

**BEAR 在校准期间会转动。在开始前，必须确保人员、衣物、电缆、工具和财产均远离全部可能运动范围，并确认转动不会造成危险。应在触手可及的位置配备独立的急停或断电手段；不得将应用内的“停止”按钮作为唯一保护措施。**

## 下载与安装

请仅从 Westwood Robotics 官网或[GitHub Releases](https://github.com/Westwood-Robotics/BEAR_Calibration_Tool/releases)等 Westwood Robotics 官方发布渠道下载安装程序。运行前，请将文件的 SHA-256与同一官方渠道公布的数值进行核对。请勿运行经第三方重新打包的安装程序。
当前 Windows x64 安装包名称和校验值见[官方 GitHub Releases 页面](https://github.com/Westwood-Robotics/BEAR_Calibration_Tool/releases)。

安装程序允许选择安装位置，并分别询问是否在 Windows 开始菜单和桌面创建名为`BEAR Calibration` 的快捷方式。使用前必须阅读并接受安装程序显示的 EULA 和安全说明。如果卸载时程序仍在运行，卸载程序会先询问是否关闭，并在确认进程已经退出后才删除文件。

## 校准数据处理方式

3.5 版本提升了受支持产品的校准精度、补偿校准可靠性，并修复了已知问题。

3.3 版本起，程序在扭矩补偿后提供摩擦补偿校准。程序在多个稳定速度下分别采集正、反转数据，
逐台拟合参数，验证通过后写入现有的校准 Flash 字段。校准结束后摩擦补偿仍保持关闭，
可由操作人员另行开启并验证。扭矩补偿现在按实际转子位置对齐正反向测量数据，以降低
摩擦带来的偏置。

从 3.2 版本开始，所有受支持产品以及 G4、F4 固件的初始 Flash 步骤均严格
只读。如果勾选“使用原 Flash 数据”且原数据有效，程序将直接使用该数据，不执行
初始写入。如果需要使用零值校准镜像，程序会先在内存中准备该镜像，并仅在流程进入
所选校准步骤后才写入。手动模式下，在用户点击“下一步”之前不会写入 Flash。

## 许可、保修与责任

本软件为闭源专有软件，按照随版本提供的 EULA 免费许可用户在个人或商业环境中用于受支持的 BEAR 产品。本许可不授予再分发、转售、再许可、托管、逆向工程或修改本软件的权利，但适用法律明确允许的情况除外。

安装后的运行时产品配置可由获授权的工程人员更新。非 Westwood Robotics提供或书面批准的数值属于用户修改，程序将按用户自担风险的方式加载，并受 EULA 及适用法律约束。

按照说明使用官方且未被修改的本软件，本身不会使原本适用的 BEAR 硬件保修失效。但在保修条款及适用法律允许的范围内，保修不涵盖因不当操作、带负载校准、未遵守说明、未经授权的参数变更或擅自修改本软件所造成的损坏。

在适用法律允许的最大范围内，用户应对由其操作、行为、不作为、修改或误用所造成的人身伤害、财产损失、设备损坏及其他损失自行承担责任，Westwood Robotics Corporation不对上述用户造成的损失承担责任。随版本提供的正式 EULA 不排除或限制适用法律不允许排除或限制的责任及消费者权利。

本版本仅由 Westwood Robotics Corporation 在美国和中国正式发布及推广。通过全球可访问的下载渠道在其他地区获取本软件，并不代表在当地进行主动营销、提供本地支持，也不代表本软件在所有司法管辖区均合法或适用。

默认情况下，每次校准保存一份精简 JSON 报告，并在适用时保存摘要图。报告包含程序
版本、产品、时间、步骤结果、旧/新最终摘要值、质量指标和错误码；默认不导出原始或
处理后的采样数据。获授权的工程人员可将安装目录中 `runtime.dat` 顶层的 `output`
设为 `1`，重启程序后，在该次校准的结果文件夹中保存详细 CSV。请将这些文件作为
设备诊断数据管理，仅在需要技术支持时分享。

## 联系方式

一般问题与安全问题：info@westwoodrobotics.io  
网站：https://www.westwoodrobotics.io/
