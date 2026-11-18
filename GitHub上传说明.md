# 最终上传步骤（维护者使用）

本目录只有 **7 个 MD 文件和 2 个组件 ZIP**。不再另套一层总 ZIP，也不需要上传旧版、分芯片 Mac 包或源码 ZIP。读者只下载适合自己电脑的一份组件包。

## 1. 更新仓库首页与教程

打开 [ResearchTrace 仓库](https://github.com/AuroraG1574/ResearchTrace)，进入 Code → Add file → Upload files，上传本目录全部 MD（或至少上传除本文件外的 6 个 MD），提交更改；若走分支流程，再合并到首页所在分支。可参考 [GitHub 上传文件说明](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository)。

## 2. 更新 Releases 附件

打开 [v0.7.0 发布页](https://github.com/AuroraG1574/ResearchTrace/releases/tag/v0.7.0)，点击编辑图标。

- 将本目录 **ResearchTrace-0.7.0-Windows.zip** 与 **ResearchTrace-0.7.0-macOS.zip** 作为附件上传。
- 发布标题建议：**研迹 ResearchTrace v0.7.0（Windows / macOS）**；正文使用本目录《发布说明.md》，包含末尾新校验值。
- 本次 Windows 也更新了包内教程，两个 ZIP 都应使用本目录的新文件。确认新附件可用后，删除当前发布页中被替代的重复旧安装附件及对应旧校验附件，避免读者选错；不要删除历史版本的其他成果。
- 如果已有同名附件，先在本地保留确认好的新文件，再在编辑页面替换同名旧附件；等上传完成后保存更新。仅修改文字不会替换附件。

若发布页已启用不可变发布，GitHub 不允许增删或替换已发布附件。此时新建发布标签 `v0.7.0-package.20261118`、上传两包，产品版本仍为 0.7.0，并将 README 的下载入口指向新发布。操作及限制见 [GitHub 发布管理说明](https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository)。

## 3. 上传后检查

1. 在未登录或无编辑权限的窗口打开发布页，确认普通读者能看到两个安装附件和说明。
2. 下载两个附件，核对文件名、大小和《发布说明.md》中的 SHA-256。
3. 解压检查安装入口和教程：Windows 为“安装研迹.cmd”，Mac 为“安装研迹.command”。
4. 保留说明中的 Mac 差异：默认浏览器工作台、未签名/公证、M4 仅确认基础启动、Intel 及完整流程待验证。不要写成 Mac 全功能或全平台验证通过。

本次已在本地整理上传材料，**没有代为上传或删除 GitHub 文件**。桌面旧压缩包的清理不影响 GitHub 已发布附件。
