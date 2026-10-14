# REA preservation

保存日期：2026-10-14。原始源码 Fork：[Nicoat/rea](https://github.com/Nicoat/rea)。

**[下载完整备份与恢复说明](https://github.com/Nicoat/rea-preservation/releases/tag/preservation-2026-10-14)**

备份保存 REA Git 历史、五个子模块完整可达历史、REA 固定版本的 LFS 实体、34 个可获取的官方 npm 发行包、6.4.0 的 552 个锁定依赖包，以及 Windows Node 运行环境、校验记录和恢复脚本。

请下载 Release 的两个自定义 ZIP，解压到同一个新目录，再阅读 `开始恢复.txt`、`README-RESTORE.md`。GitHub 自动生成的 Source code ZIP 仅包含本仓库的归档工具，REA 实际源码在自定义备份附件中。

`.github/workflows/preserve.yml` 只接受手动触发；它从固定白名单下载地址重建并核验备份，不执行 REA 或 npm 包代码。原始源码 Fork 的工作流保持禁用。`transfer-seed.zip` 保存原始元数据、校验信息和归档助手；它不是 REA 安装包。

这是固定快照。独立分析引擎、商业许可及 AI 服务需另行准备。所有原始版权和许可保留在各组件中。
