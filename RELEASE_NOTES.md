## 关闭窗口磨砂的 Intel Mac 测试版

基于 DeepSeek Harness **0.2.1-rc.4**，关闭主窗口原生磨砂（`vibrancy`）和透明背景，改用实色背景。

该测试版用于尝试降低 Intel 芯片 Mac 上与 `VRR_ERR` 相关的屏幕渲染超时、黑屏和异常重启／退回登录界面问题。**实际缓解效果尚未验证，`VRR_ERR` 与这些现象的因果关系也尚未确定。** 这是非官方、本机临时签名的对照测试程序。

### 附件

- **DSH Opaque Window Test.zip**：现有 ZIP 压缩包。
- **DSH-Opaque-Window-Test-macOS-x64.app.tar.gz**：`.app` 程序目录包的归档。
- **SHA256SUMS.txt**：上述两个附件的 SHA-256 校验值。

两个程序附件包含同一测试版，任选其一下载并解压即可。平台为 **macOS Intel / x86_64**，程序声明最低系统版本为 **macOS 13.0**。

### 使用

先保存工作并用 `⌘Q` 退出其他 DSH 实例，再打开解压后的 `DSH Opaque Window Test.app`。测试版使用独立数据目录：

```text
~/Library/Application Support/DSH Opaque Window Test/
```

测试时保持其他系统图形设置一致；如果问题复发，记录时间、操作和实际现象，并保留系统诊断资料。详细改动和操作说明见仓库 README。
