<!--
Copyright Advanced Micro Devices, Inc.

SPDX-License-Identifier: MIT
-->

<!-- @device:halo,stx,krk,rx7900xt,rx9070xt,r9700 -->
<!-- @os:windows -->
### AMD GPU Driver

使用 [`AMD Software: Adrenalin Edition™`](https://www.amd.com/en/products/software/adrenalin.html) 更新到最新 AMD GPU driver。

1. 从开始菜单或系统托盘打开 `AMD Software: Adrenalin Edition`。
2. 进入 **Driver and Software**，点击 **Manage Updates**。
3. 如果有可用更新，请按照提示下载并安装。

<!-- @test:id=amd-gpu-visible-windows timeout=60 hidden=True -->
```powershell
Get-CimInstance Win32_VideoController | Select-Object Name, DriverVersion
```
<!-- @test:end -->
<!-- @os:end -->
<!-- @device:end -->

<!-- @os:linux -->
<!-- @device:rx7900xt,rx9070xt,r9700 -->
### AMD GPU Driver

使用 Radeon Software for Linux (RSL) 流程安装 AMD GPU Driver (amdgpu)。有关你的发行版的安装说明，请参阅 [Install the kernel driver](https://rocm.docs.amd.com/en/7.13.0-preview/install/rocm.html)。

<!-- @device:end -->
<!-- @os:end -->
