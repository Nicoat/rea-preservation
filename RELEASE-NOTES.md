这是一份个人保存快照，原始源码 Fork 为 [Nicoat/rea](https://github.com/Nicoat/rea)。

保存内容：
- REA 的 106 分支、35 个原始标签及完整可达 Git 历史。
- 5 个子模块完整可达 Git 历史，以及 892 个 REA 固定版本的 unblob LFS 实体。
- 34 个可获取的官方新旧 npm 发行包、正式版 6.4.0 的 552 个锁定依赖包。
- Node.js 24.18.0 Windows x64、35 个上游 Release 记录、校验清单、中英文恢复说明和恢复脚本。

下载两个自定义 ZIP 并解压到同一个新目录。先按 SHA256SUMS.txt 检查压缩包，再运行 `python verify_archive.py` 验证全部内容。源码恢复：`python restore_sources.py --output ../rea-restored --ref rea-agents-6.4.0`。已构建发行包的恢复步骤见 `npm/RESTORE-npm.txt`。

已完成本地 Git/LFS 恢复、禁用安装脚本的离线 npm 依赖恢复；GitHub 端再次核对每个归档文件及四个上传附件的 SHA256。没有运行 REA 功能测试。

范围限制：npm 2.5.1、2.6.0、2.7.0 当前不可获取，其 Git 源码已保存。unblob 的其他历史 LFS 和各旧版的依赖环境未全部镜像。Windows 下 unblob/tests 的特殊文件名通过稀疏工作区处理，完整 Git/LFS 数据仍保留。外部引擎、商业许可及 AI 服务需另行准备。

该 npm ZIP 在 GitHub 直接从原始地址重建，因此压缩包外层校验值与初始本地压缩包不同；内部 597 个文件与本地已验证快照逐字节一致。请以本页附带的 SHA256SUMS.txt 为准。
