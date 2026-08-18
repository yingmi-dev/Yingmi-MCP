# 盈米 MCP Server

盈米 MCP Server 是一个基于模型上下文协议（MCP）的智能投资顾问服务，为 AI 助手提供专业的基金分析、资产配置、投资组合诊断等金融服务能力。通过自然语言交互，让投资决策更智能、更高效。产品注册、介绍与开放平台入口见 **[盈米 AI开放平台](https://ai.yingmi.com)**；API Key 与接入详情请以平台内控制台为准。

## 核心能力

### 📊 资产与家庭财务分析

- **资产负债分析**：智能计算资产负债比率、净资产等核心财务指标
- **现金流分析**：基于家庭收支与资产配置生成现金流健康度报告
- **家庭成员分析**：统计家庭人数与生命周期阶段，提供定制化建议
- **财务指标诊断**：评估关键财务指标的合理性，识别潜在风险
- **收支结构分析**：可视化年度收支分布与占比，优化财务规划

### 💼 基金与组合分析

- **基金风险评估**：多维度风险评分与指标分析（波动率、最大回撤、夏普比率等）
- **组合风险诊断**：基金组合整体风险评估与优化建议
- **持仓诊断**：深度分析基金配置合理性、相关性与历史回测表现
- **资产配置分析**：基金组合资产大类穿透，识别隐藏风险
- **相关性分析**：发现基金间的相关性，避免过度集中
- **回测模拟**：历史数据回测与蒙特卡洛模拟，测算不同情景下的潜在收益与风险区间

### 🔍 基金信息查询

- **基金详情**：批量获取基金净值、业绩、费率、交易规则等全面信息
- **业绩诊断**：估值水平、业绩归因分析
- **智能搜索**：支持基金名称模糊匹配、多维度筛选排序
- **热门基金**：获取近期热门基金与市场关注趋势
- **交易规则查询**：及时获取基金交易规则、申赎限额等关键信息

### 📈 专业投资分析

- **行业配置分析**：基金行业偏好、集中度与收益贡献分析
- **债券指标**：久期、杠杆、信用评级等债券基金专业指标
- **股票指标**：权益仓位、换手率、择时能力、Brinson归因分析
- **QDII分析**：海外基金地区配置与风险评估
- **策略研究**：基金策略详情、风险信息与资产穿透

### 🛠️ 辅助工具

- **数据可视化**：ECharts 图表渲染，直观展示分析结果
- **报告生成**：HTML 转 PDF，一键生成专业投资报告
- **实时资讯**：财经新闻、热点话题、基金经理观点搜索
- **AI 解读**：实时 AI 资讯解读与投顾内容推荐

## 适用场景

### 个人投资者

- 快速诊断现有基金组合的风险与收益特征
- 获取专业的资产配置建议与优化方案
- 追踪市场热点与基金经理最新观点

### 投资顾问

- 为客户提供专业的财务规划与资产配置服务
- 批量分析基金产品，快速生成投资报告
- 查询与评估组合风险，为投资策略调整提供参考

### 金融研究员

- 深度分析基金业绩归因与风险来源
- 研究行业配置趋势与市场轮动规律
- 回测投资策略，验证投资逻辑

## 完整工具清单（69）

### 金融数据（35）

#### 基金数据（28）

- SearchFunds - 搜索基金
- BatchGetFundNavHistory - 基金净值历史
- BatchGetFundsDetail - 批量获取基金详情
- GetBatchFundPerformance - 批量获取基金业绩表现
- AnalyzeFundRisk - 基金风险分析
- BatchGetFundTradeLimit - 基金交易限制信息
- BatchGetFundsDividendRecord - 基金分红记录
- fund-equity-position - 权益仓位偏好
- getFundIndustryAllocation - 行业配置比例
- BatchGetFundTradeRules - 基金交易规则
- getFundTurnoverRate - 基金换手率（调仓频率）
- getFundBenchmarkInfo - 基金业绩基准
- getStockAllocationAndMetricsByFundCode - 估值盈利指标（市盈率/市净率/净资产收益率）
- getFundBrinsonIndicator - Brinson归因
- GetFundAssetClassAnalysis - 资产大类分布
- getBondIndicator - 债基风险
- fund-recovery-ability - 回撤修复能力
- getFundIndustryConcentration - 基金行业持仓集中度
- getFundIndustryReturns - 行业收益
- getFundCampisiIndicator - Campisi归因
- getBondAllocationByFundCode - 券种配置情况
- getFundIndustryPreference - 基金行业偏好
- fund-sector-preference - 基金板块偏好
- getQdFundAreaAllocation - QDII地区配置
- getMarketTimingIndicator - 权益仓位择时
- BatchGetFundsSplitHistory - 基金拆分记录
- getFundDiveCount - 债基异动
- getBondFundCreditRatingLevel - 债基评级查询

#### 策略数据（7）

- GetStrategyDetails - 策略详情查询
- GetStrategyAssetClassAnalysis - 策略大类资产分布
- BatchGetStrategiesComposition - 批量查询策略持仓
- GetStrategyRiskInfo - 策略风险
- GetStrategyBenchmark - 查询策略业绩基准
- GetPortfolioNavHistory - 组合历史净值
- BatchGetPoTradeComposition - 策略交易成分

### 投研服务（13）

#### 投前分析（8）

- GetFundDiagnosis - 基金诊断
- GetPopularFund - 获取近期热门基金
- GetLatestQuotations - 市场温度计
- GetFundRelatedStrategies - 按重仓基金筛选投顾策略
- getBondFundWithAlertRecord - 查询发生净值异动的债基
- filterBondFundByBondType - 券种风格筛选基金
- filterBondFundByCreditRating - 根据信用评级筛选基金
- filterStockFundByStockTurnover - 股票换手率筛选基金

#### 测算能力（2）

- GetFundsBackTest - 回测分析
- MonteCarloSimulate - 组合预期收益测算（蒙特卡洛）

#### 投后诊断（3）

- AnalyzePortfolioRisk - 投后风险分析
- GetFundsCorrelation - 基金相关性分析
- GetAssetAllocation - 资产配置分析

### 通用服务（5）

#### 金融工具（1）

- GuessFundCode - 基金代码模糊匹配

#### 常用工具（4）

- GetCurrentTime - 获取当前时间
- RenderEchart - ECharts图表渲染
- RenderHtmlToPdf - HTML转PDF
- GetTxnDayRange - 交易日查询

### 投顾服务（11）

#### 投资顾问（11）

- GetAssetAllocationPlan - 获取资产配置方案
- StrategySearchByKeyword - 策略关键词搜索
- AnalyzeFinancialIndicators - 财务状况分析
- DiagnoseFundPortfolio - 账户诊断
- GetCompositeModel - 获取基金投资方案
- BatchGetStrategyRiskInfo - 策略风险匹配
- AnalyzeInvestmentPerformance - 投资方案表现分析
- AnalyzeFamilyMembers - 家庭结构分析
- AnalyzeCashFlow - 现金流分析与财务规划
- AnalyzeAssetLiability - 资产负债分析
- AnalyzeIncomeExpense - 收入支出分析接口

### 投顾内容（5）

#### 公开内容（2）

- SearchFinancialNews - 财经资讯
- SearchHotTopic - 热点财经话题榜单

#### 盈米生产（3）

- SearchManagerViewpoint - 基金经理观点
- searchInvestAdvisorContent - 搜索投顾内容
- searchRealtimeAiAnalysis - 实时资讯AI解读

## 快速开始

### 接入方式：云托管（Streamable HTTP）

盈米 MCP Server 采用 **云托管模式**，无需本地部署服务端代码。通过 **Streamable HTTP**（MCP 当前推荐的 HTTP 传输；客户端中的具体名称可能略有不同）接入。

**接入地址**：`https://stargate.yingmi.com/mcp/v2`（鉴权使用请求头 **`x-api-key`**，并建议设置 **`Accept: application/json, text/event-stream`**）

> **以控制台为准**：[盈米AI开放平台——个人中心](https://ai.yingmi.com/mcp/account) 会展示与您账号对应的接入方式与完整 URL；**若页面与本文示例不一致，请以平台控制台为准。**

### 步骤 1：获取 API Key

1. 打开 [盈米 AI开放平台](https://ai.yingmi.com) 完成注册并了解服务
2. 登录后在 [盈米AI开放平台——个人中心](https://ai.yingmi.com/mcp/account) 申请并复制 MCP API Key
3. 妥善保存 API Key（后续配置时需要）

> 💡 **提示**：更多说明与 Key 管理以 [盈米 AI开放平台](https://ai.yingmi.com) 及 [盈米AI开放平台——个人中心](https://ai.yingmi.com/mcp/account) 为准。

### 步骤 2：在 Claude Code 中配置

Claude Code 已原生支持远程 HTTP MCP，无需使用 `mcp-remote`。推荐在项目根目录创建 `.mcp.json`，并通过环境变量注入 API Key：

```json
{
  "mcpServers": {
    "qieman": {
      "type": "http",
      "url": "https://stargate.yingmi.com/mcp/v2",
      "headers": {
        "x-api-key": "${YINGMI_API_KEY}",
        "Accept": "application/json, text/event-stream"
      }
    }
  }
}
```

使用前先设置 `YINGMI_API_KEY` 环境变量，并重新启动 Claude Code。也可用命令行直接添加：

```powershell
claude mcp add --transport http --scope user qieman https://stargate.yingmi.com/mcp/v2 --header "x-api-key: your-api-key-here" --header "Accept: application/json, text/event-stream"
```

> 命令行方式会把请求头写入 Claude Code 配置；若不希望 Key 明文落盘，请使用上面的 `.mcp.json` + 环境变量方案。可运行 `claude mcp list`，或在 Claude Code 中输入 `/mcp` 检查连接状态。

### 步骤 3：在 Claude Desktop 中配置

Claude Desktop 的 **Connectors（连接器）** 适用于支持 OAuth 或无需鉴权的远程 MCP。当前盈米 MCP 需要自定义 `x-api-key` 请求头，不能仅填写 URL 直接接入 Connectors；请使用 `mcp-remote` 作为本地 stdio 兼容桥接。若盈米 AI 开放平台后续提供 OAuth 兼容的 Connector 地址，再以控制台说明为准改用 **设置 → Connectors → Add custom connector**。

#### Claude Desktop + mcp-remote（兼容方案）

在 Claude Desktop 配置文件中添加（需安装 Node.js，`mcp-remote` 需支持 Streamable HTTP）：

```json
{
  "mcpServers": {
    "qieman": {
      "command": "npx",
      "args": [
        "-y",
        "mcp-remote",
        "https://stargate.yingmi.com/mcp/v2",
        "--transport",
        "http-only",
        "--header",
        "x-api-key:${YINGMI_API_KEY}",
        "--header",
        "Accept:${MCP_ACCEPT}"
      ],
      "env": {
        "YINGMI_API_KEY": "your-api-key-here",
        "MCP_ACCEPT": "application/json, text/event-stream"
      }
    }
  }
}
```

**配置说明**：

- 该配置注册的是本地 stdio 桥接进程，而不是在 `claude_desktop_config.json` 中直接注册远程 HTTP Server
- `mcp-remote` 将远程 Streamable HTTP MCP 桥接为本地 stdio，供 Claude Desktop 使用
- 将 `env.YINGMI_API_KEY` 中的 `your-api-key-here` 替换为您的真实 API Key
- Windows 下请求头参数不包含空格；带空格的完整值通过 `env` 注入，避免 Claude Desktop 调用 `npx` 时错误拆分参数
- 此兼容配置会将 Key 保存在本地 Claude Desktop 配置文件中，请勿提交到 Git，并注意限制文件访问权限

> 保存后重启 Claude Desktop。若连接失败，请先核对 API Key 和服务地址，再升级 `mcp-remote`，并检查 Claude Desktop 的 MCP 日志。

### 步骤 4：在其他 MCP 客户端中使用

#### Cursor IDE

**配置步骤**：

1. 打开 Cursor，进入**设置**
2. 打开 **MCP**
3. **添加 MCP Server**，填入下列配置并保存

**Streamable HTTP**：

```json
{
  "mcpServers": {
    "qieman": {
      "url": "https://stargate.yingmi.com/mcp/v2",
      "headers": {
        "x-api-key": "your-api-key-here",
        "Accept": "application/json, text/event-stream"
      }
    }
  }
}
```

**配置说明**：

- 将 `headers` 中的 `your-api-key-here` 替换为您的实际 API Key；`Accept` 建议保持与上例一致
- 若 Cursor 提供传输类型选项，请选择 **Streamable HTTP**（或 HTTP）以匹配上述配置
- Cursor 下载：[https://www.cursor.com/cn](https://www.cursor.com/cn)

#### Codex（CLI / IDE）

Codex CLI 与 IDE 扩展通过 `~/.codex/config.toml` 配置远程 MCP。Windows 路径一般为 `%USERPROFILE%\.codex\config.toml`。ChatGPT 网页端不会读取此本地配置。

```toml
[mcp_servers.qieman]
url = "https://stargate.yingmi.com/mcp/v2"
env_http_headers = { "x-api-key" = "YINGMI_API_KEY" }
http_headers = { "Accept" = "application/json, text/event-stream" }
```

**配置说明**：

- 使用前先设置 `YINGMI_API_KEY` 环境变量，并重新启动 Codex
- `env_http_headers` 的值是环境变量名称，不是 API Key 本身；不要再在 `http_headers` 中重复配置明文 `x-api-key`
- 配置参考：[Codex config.toml](https://learn.chatgpt.com/docs/config-file/config-reference)
- 也可用 `codex mcp add qieman --url https://stargate.yingmi.com/mcp/v2` 先写入地址，再在 `config.toml` 中补充上述 headers

#### Cherry Studio

在连接类型中选择 **HTTP / Streamable HTTP**（名称以软件为准），服务器地址填 `https://stargate.yingmi.com/mcp/v2`，并在自定义请求头中设置 **`x-api-key`**（值为您的 API Key）及 **`Accept: application/json, text/event-stream`**（若软件支持填写 headers）。

**配置说明**：

- Cherry Studio 下载：[https://www.cherryai.com.cn/](https://www.cherryai.com.cn/)

#### Windsurf / Trae 等其他 IDE

**Streamable HTTP**（与 Cursor 相同，需支持 `headers` 配置）：

```json
{
  "mcpServers": {
    "qieman": {
      "url": "https://stargate.yingmi.com/mcp/v2",
      "headers": {
        "x-api-key": "your-api-key-here",
        "Accept": "application/json, text/event-stream"
      }
    }
  }
}
```

> ⚠️ **兼容性说明**：不同客户端对 MCP 传输（Streamable HTTP）的支持可能不同；**请以客户端文档及 [盈米 AI开放平台](https://ai.yingmi.com) 控制台信息为准。**

### 使用示例

**场景1：诊断基金组合**

```
我持有以下基金：易方达蓝筹精选(005827)、兴全合润(163406)、中欧时代先锋(001938)，请帮我分析组合的风险和相关性。
```

**场景2：资产配置建议**

```
我有100万资金，风险承受能力中等，希望年化收益8%左右,请帮我设计一个资产配置方案。
```

**场景3：业绩归因分析**

```
基于Campisi模型，拆解基金代码为001001的华夏债券基金A类在2025年6月30日到9月30日的总收益中，利率变动、信用利差变化、息票收入及其他因素各自的贡献比例是多少？
```

## 技术特点

- **云托管服务**：无需本地部署服务端代码，在客户端配置 **Streamable HTTP** 接入地址即可使用
- **专业可靠**：基于盈米投顾多年积累的金融数据与分析模型
- **数据更新**：支持获取最新基金净值与市场资讯
- **智能分析**：结合 AI 能力，提供自然语言交互式投资分析
- **可视化**：内置图表渲染与报告生成能力，结果一目了然
- **标准协议**：基于 MCP 协议，兼容 Claude Desktop、Cursor、Trae 等主流 AI 工具
- **安全可控**：API Key 认证，数据传输加密，保障信息安全

## 免责声明

本服务提供的所有信息、分析与建议仅供参考，不构成任何投资建议或承诺。投资有风险，决策需谨慎。使用本服务产生的任何投资损失，开发者与服务提供方不承担责任。请在充分了解风险的前提下，结合自身情况做出投资决策。

## 开源协议

MIT License

## 联系方式

- 问题反馈: [wangjiaye@yingmi.cn](mailto:wangjiaye@yingmi.cn)
- GitHub: [Yingmi-MCP](https://github.com/yingmi-dev/Yingmi-MCP)
- 开放平台: [盈米 AI开放平台](https://ai.yingmi.com)

---

**由盈米提供专业金融数据支持**
