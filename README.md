# DALI Toolkit · 客户下载

**用自然语言，让 AI 帮你调灯、编排场景和整理 DALI 工程。**

当前稳定版 **0.47**。适用于 Windows、兼容网关，以及支持本地 MCP 的 AI 客户端。

## 把这段话发给你的 AI

首次安装：

> 请安装 https://github.com/appleyancheng-art/Dali-Toolkit 。先读 AGENTS.md，再按 INSTALL.md 安装稳定版 MCP 和两个 Skill，完成离线检查并接入我当前使用的客户端。已有配置和数据要保留；安装时不要操作灯具。

以后更新：

> 请更新当前客户端的 DALI Toolkit：https://github.com/appleyancheng-art/Dali-Toolkit 。只先读 release.json 和 UPDATE.md。保留原配置、数据和旧版本，接着尚未完成的一步处理，不重复安装已准备好的同版本。完成 MCP 入口切换、正常重载、实际版本核对和两个 Skill 更新；不要操作灯具、刷固件或改其他客户端。

AI 需要具备本机文件操作、运行程序和管理 MCP 的能力。只有网页聊天或只支持远程 MCP 的客户端，不能直接启动本套件。详见[使用条件](COMPATIBILITY.md)。

## 可以帮你做什么

| 你想做的事 | Toolkit 提供的能力 |
| --- | --- |
| 到新项目开始调试 | 搜索局域网网关，读取灯具与当前状态 |
| 调整灯光 | 指定单灯、多个灯或灯组的亮度、色温，开关与找灯 |
| 设计场景 | 先看实时效果，再保存；支持不同灯使用不同参数、批量场景和图案编排 |
| 配置设备 | 分组、渐变、亮度及色温范围、上电和故障输出等参数 |
| 管理地址 | 改址、删除短地址、自动新增、交换、全量寻址、通道重置 |
| 整理交付 | 工程备份、比较和受支持配置恢复，Excel、名称备注与平面图资料 |

[查看完整功能与适用范围](FUNCTIONS.md) · **[各功能调试提示词：直接复制使用](PROMPTS.md)** · [第一次使用](GET-STARTED.md) · [常见问题](FAQ.md)

## 下载

**[下载 0.47 主安装包：MCP + 两个 Skill](https://raw.githubusercontent.com/appleyancheng-art/Dali-Toolkit/main/packages/0.47-customer.2/DALI-Toolkit-0.47-customer.2.zip)**

通常只需这个 ZIP。请交给 AI 按上面的安装流程处理；解压不等于安装完成，也不是双击即用的独立桌面 App。

| 单独下载 | 用途 |
| --- | --- |
| [MCP 调试 Skill](https://raw.githubusercontent.com/appleyancheng-art/Dali-Toolkit/main/packages/0.47-customer.2/dali-mcp-control-0.47.zip) | 指导 AI 直接使用网关 MCP；仍需要已安装的 MCP 服务 |
| [上位机操作 Skill](https://raw.githubusercontent.com/appleyancheng-art/Dali-Toolkit/main/packages/0.47-customer.2/dali-config-computer-use-0.47.zip) | 指导 AI 操作 DALI Config Tool；需要客户端另有 Computer Use 能力与厂家软件 |
| [SHA256 校验值](SHA256SUMS.txt) | 核对下载文件是否完整一致 |

下载文件由本客户仓库直接提供，版本与校验值见 [release.json](release.json)。**不要点击 GitHub 的“Download ZIP”代替安装包。**

## 开始调试

**[打开完整调试提示词库](PROMPTS.md)**：24 类功能，每类多个例子，涵盖网关、调灯、场景、分组、九类参数、六项地址管理、工程、Excel、平面图和上位机界面操作。

安装验证完成后，可以这样说：

> 搜索当前局域网的 DALI 网关，列出来让我选，然后读取通道 B 的灯具。

> 把通道 B 地址 0、63 调到 100%、4000K，其他灯保持，先预览。

> 这个效果可以，把刚才指定的两盏灯保存到场景 6。

地址为 **0–63**，场景和组为 **0–15**；“场景 8”就是上位机的场景 8。新现场先搜索网关，不沿用别人的 IP。

## 版本与帮助

[版本变化](CHANGELOG.md) · [安装流程（给 AI）](INSTALL.md) · [更新流程（给 AI）](UPDATE.md) · [问题反馈](SUPPORT.md)

当前交付为 Windows MCP 和两个 Skill。iOS App 尚未发布；本版不需要授权码。
