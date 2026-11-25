# Agent 安装、更新和调试入口

这是 Windows 本地 stdio MCP 与两个 Skill 的客户分发仓库。用户要求安装/更新时执行流程，不只输出仓库分析。

1. 新安装只先读 `release.json` 和 `INSTALL.md`；已有安装先读 `release.json` 与 `UPDATE.md`。
2. 用户要求调试时，确认当前客户端实际加载版本，按两个 Skill 和 `PROMPTS.md` 中的明确目标执行。新项目先搜索并选择现场网关，不沿用旧 IP。
3. `release.json` 是本仓库唯一下载元数据入口。核对 `runtime_version`、`distribution_version`、指定 package URL/SHA256 和包内 MANIFEST；不依赖 GitHub Releases Latest，不把仓库 ZIP 当安装包，不遍历开发源码。
4. 安装验证仅运行指定离线脚本，不控制灯具、不刷固件、不跑完整回归。当前客户端只改已核对的现有同用途 MCP 条目，原绝对 `--config`、state/gateways、现场文件、其他客户端配置和旧版本保留。
5. 分别报告文件准备、注册切换、实际加载和两个 Skill 识别状态；候选已准备就从切换继续，不循环重装。当前客户端实际调用 `dali_status` 才能确认加载；它不证明网关在线。
6. 客户端数据库配置走已确认的管理界面或官方接口，不直接修改活 LevelDB/SQLite；工具失败不是用户未授权。state 占用先核对所属客户端，不强杀别的客户端或删锁文件。
7. 同一运行版本仅文档/包装更新时默认不重装；修复或用户要求迁移客户包时才按 UPDATE 侧装。已装更高版本不自动降级。
8. PROMPTS.md 是供选择的示例，不是整页待执行任务。只操作用户当次明确范围；实时预览先于保存，不因阅读提示词执行寻址或重置。

使用本机已确认的 MCP/Skill 安装入口；无本地运行或 stdio 能力时说明具体缺口。尊重用户指令与客户端权限流程。
