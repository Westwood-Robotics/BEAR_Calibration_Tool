# BEAR Calibration Tool

BEAR Calibration Tool is the official Windows calibration utility for supported BEAR actuators from Westwood Robotics Corporation. BEAR products are calibrated before shipment and normally do not require this utility. It is provided free of charge for exceptional recovery, service, or recalibration situations.

## Critical safety warning

**Before every calibration, completely remove every external load from the BEAR actuator. Disconnect its output from every robot, linkage, transmission, tool, fixture, and other mechanism. Secure the actuator body and confirm that the output shaft can rotate freely.**

**The BEAR actuator will rotate during calibration. Do not begin until all people, clothing, cables, tools, and property are outside its full possible motion area and the movement cannot create a hazard. Keep an independent emergency-stop or power-disconnect method within reach. Do not rely on the application's Stop button as the only protective measure.**

## Download and installation

Download the installer only from an official Westwood Robotics distribution channel: the [company website](https://www.westwoodrobotics.io/) or the official [GitHub Releases](https://github.com/Westwood-Robotics/BEAR_Calibration_Tool/releases).

Before running it, compare the file's SHA-256 value with the value published through the same official channel. Do not run a repackaged or third-party installer.

The installer lets you select the installation directory and separately choose whether to create `BEAR Calibration` shortcuts on the Windows Start Menu and desktop. Read and accept the displayed EULA and safety information before use. If the application is running when uninstall starts, the uninstaller asks before requesting a normal close and does not remove files until the process has exited.

## License, warranty, and responsibility

The Software is proprietary and closed source. It is licensed free of charge for personal and commercial use with supported BEAR products, subject to the EULA supplied with the release. The license does not grant rights to redistribute, resell, sublicense, host, reverse engineer, or modify the Software except where applicable law expressly permits otherwise.

The installed runtime product configuration can be updated by authorized engineering personnel. Values not supplied or expressly approved by Westwood Robotics are user modifications and are loaded at the user's own risk, subject to the EULA and applicable law.

Use of the official, unmodified Software according to its instructions does not, by itself, void an otherwise applicable BEAR hardware warranty. Subject to the warranty terms and applicable law, damage caused by improper operation, calibration while loaded, failure to follow instructions, unauthorized parameter changes, or modification of the Software is not covered by warranty.

To the maximum extent permitted by applicable law, the user is responsible for bodily injury, property damage, equipment damage, and other loss caused by the user's operation, acts, omissions, modifications, or misuse. Westwood Robotics Corporation does not accept liability for such user-caused loss. The controlling EULA preserves any liability and consumer rights that applicable law does not permit the parties to exclude or limit.

Official publication and marketing of this release are limited to the United States and China. Technical availability through a globally accessible download channel does not represent active marketing, local support, legality, or suitability in every jurisdiction.

Each calibration session saves one concise JSON report and, where applicable, summary plots. The report contains version, product, timestamps, step outcomes, old/new final summary values, quality metrics, and error codes. Raw and processed samples, complete coefficient sets, and complete torque tables are not exported.

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

安装程序允许选择安装位置，并分别询问是否在 Windows 开始菜单和桌面创建名为`BEAR Calibration` 的快捷方式。使用前必须阅读并接受安装程序显示的 EULA 和安全说明。如果卸载时程序仍在运行，卸载程序会先询问是否关闭，并在确认进程已经退出后才删除文件。

## 许可、保修与责任

本软件为闭源专有软件，按照随版本提供的 EULA 免费许可用户在个人或商业环境中用于受支持的 BEAR 产品。本许可不授予再分发、转售、再许可、托管、逆向工程或修改本软件的权利，但适用法律明确允许的情况除外。

安装后的运行时产品配置可由获授权的工程人员更新。非 Westwood Robotics提供或书面批准的数值属于用户修改，程序将按用户自担风险的方式加载，并受 EULA 及适用法律约束。

按照说明使用官方且未被修改的本软件，本身不会使原本适用的 BEAR 硬件保修失效。但在保修条款及适用法律允许的范围内，保修不涵盖因不当操作、带负载校准、未遵守说明、未经授权的参数变更或擅自修改本软件所造成的损坏。

在适用法律允许的最大范围内，用户应对由其操作、行为、不作为、修改或误用所造成的人身伤害、财产损失、设备损坏及其他损失自行承担责任，Westwood Robotics Corporation不对上述用户造成的损失承担责任。随版本提供的正式 EULA 不排除或限制适用法律不允许排除或限制的责任及消费者权利。

本版本仅由 Westwood Robotics Corporation 在美国和中国正式发布及推广。通过全球可访问的下载渠道在其他地区获取本软件，并不代表在当地进行主动营销、提供本地支持，也不代表本软件在所有司法管辖区均合法或适用。

每次校准仅保存一份精简 JSON 报告，并在适用时保存摘要图。报告包含程序版本、产品、时间、步骤结果、旧/新最终摘要值、质量指标和错误码；不导出原始或处理后采样、完整系数集合或完整扭矩补偿表。

## 联系方式

一般问题与安全问题：info@westwoodrobotics.io  
网站：https://www.westwoodrobotics.io/
