# 且慢 MCP Server

且慢 MCP Server 是一个基于模型上下文协议（MCP）的智能投资顾问服务，为 AI 助手提供专业的基金分析、资产配置、投资组合诊断等金融服务能力。通过自然语言交互，让投资决策更智能、更高效。

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
- **回测模拟**：历史数据回测与蒙特卡洛模拟，预测未来收益区间

### 🔍 基金信息查询

- **基金详情**：批量获取基金净值、业绩、持仓、费率等全面信息
- **业绩诊断**：估值水平、业绩归因分析
- **智能搜索**：支持基金名称模糊匹配、多维度筛选排序
- **热门基金**：实时追踪市场热门基金与投资趋势
- **公告查询**：及时获取基金公告、交易规则、限额信息

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
- 实时监控组合风险，及时调整投资策略

### 金融研究员

- 深度分析基金业绩归因与风险来源
- 研究行业配置趋势与市场轮动规律
- 回测投资策略，验证投资逻辑

## 完整工具清单

## 资产与家庭财务分析（5）

- AnalyzeAssetLiability - 资产负债分析
- AnalyzeCashFlow - 现金流分析
- AnalyzeFamilyMembers - 家庭成员分析
- AnalyzeFinancialIndicators - 财务指标分析
- AnalyzeIncomeExpense - 收入支出分析

## 基金与组合分析（8）

- AnalyzeFundRisk - 基金风险分析
- AnalyzePortfolioRisk - 组合风险评估
- DiagnoseFundPortfolio - 基金持仓诊断
- GetAssetAllocation - 资产配置分析
- GetFundAssetClassAnalysis - 资产大类穿透
- GetFundsBackTest - 组合回测
- GetFundsCorrelation - 相关性分析
- MonteCarloSimulate - 蒙特卡洛模拟

## 基金信息查询（7）

- BatchGetFundNavHistory - 批量获取历史净值
- BatchGetFundsDetail - 批量获取基金详情
- GetBatchFundPerformance - 批量业绩表现
- GetFundDiagnosis - 基金诊断
- SearchFunds - 基金搜索
- GetPopularFund - 热门基金
- GuessFundCode - 基金代码模糊匹配

## 持仓特征与能力评价（7）

- fund-sector-preference - 板块偏好
- fund-equity-position - 权益仓位偏好
- fund-recovery-ability - 回撤修复能力
- getFundTurnoverRate - 基金换手率（调仓频率）
- getFundIndustryPreference - 行业偏好
- getFundIndustryAllocation - 行业配置比例
- getFundIndustryConcentration - 行业持仓集中度

## 基金持仓 / 归因 / 风险细分（14）

- getQdFundAreaAllocation - QDII 地区配置
- getBondFundCreditRatingLevel - 债基评级分布
- getBondAllocationByFundCode - 券种配置情况
- getStockAllocationAndMetricsByFundCode - 重仓股与估值指标分析
- getFundIndustryReturns - 行业收益
- getFundBrinsonIndicator - Brinson 归因
- getMarketTimingIndicator - 权益仓位择时
- getFundCampisiIndicator - Campisi 归因
- getBondIndicator - 债基风险指标（杠杆/久期/集中度）
- getFundDiveCount - 债基异动
- filterBondFundByCreditRating - 信用评级筛选基金
- filterBondFundByBondType - 券种风格筛选基金
- filterStockFundByStockTurnover - 股票换手率筛选基金
- getBondFundWithAlertRecord - 查询发生净值异动的债基

## 基本信息与交易规则（6）

- getFundBenchmarkInfo - 业绩基准（合同基准）
- BatchGetFundTradeRules - 基金交易规则
- BatchGetFundTradeLimit - 基金交易限制信息
- BatchGetFundsSplitHistory - 基金拆分记录
- BatchGetFundsDividendRecord - 基金分红记录
- BatchGetFundsHolding - 基金持仓

## 策略与投顾（9）

- GetStrategyDetails - 策略详情查询
- GetStrategyBenchmark - 查询策略业绩基准
- GetStrategyAssetClassAnalysis - 策略大类资产分布
- BatchGetStrategiesComposition - 批量查询策略持仓
- BatchGetPoTradeComposition - 策略交易成分
- StrategySearchByKeyword - 策略关键词搜索
- BatchGetStrategyRiskInfo - 批量策略风险匹配
- GetStrategyRiskInfo - 策略风险查询
- GetFundRelatedStrategies - 按重仓基金筛选投顾策略

## 资讯与公告（7）

- SearchFinancialNews - 财经资讯
- SearchManagerViewpoint - 基金经理观点
- searchRealtimeAiAnalysis - 实时资讯 AI 解读
- SearchHotTopic - 热点财经话题榜单
- searchInvestAdvisorContent - 搜索投顾内容
- GetFundAnnouncements - 查询基金公告
- GetAnnouncementContent - 获取公告内容

## 投资规划与组合（4）

- GetAssetAllocationPlan - 获取资产配置方案
- GetCompositeModel - 获取基金投资方案
- AnalyzeInvestmentPerformance - 投资方案表现分析
- GetPortfolioNavHistory - 组合历史净值

## 市场与辅助工具（5）

- GetLatestQuotations - 市场温度计
- RenderEchart - 图表渲染
- RenderHtmlToPdf - 报告生成
- GetCurrentTime - 时间工具
- GetTxnDayRange - 交易日查询

## 快速开始

### 接入方式：云托管（Streamable HTTP / SSE）

且慢 MCP Server 采用 **云托管模式**，无需本地部署服务端代码。支持两种传输（具体名称以客户端为准）：


| 传输方式                | 说明                                                                    |
| ------------------- | --------------------------------------------------------------------- |
| **Streamable HTTP** | MCP 当前推荐的 HTTP 传输；适合已原生支持该传输的客户端（如新版 Cursor）。                         |
| **SSE**             | 传统 SSE 长连接；兼容面广，**Claude Desktop 等仅支持 stdio 的环境**需通过 `mcp-remote` 桥接。 |


**接入地址**：

- **Streamable HTTP**：`https://stargate.yingmi.com/mcp/v2`（鉴权使用请求头 `**x-api-key`**，并建议设置 `**Accept: application/json, text/event-stream`**）
- **SSE**：`https://stargate.yingmi.com/mcp/sse?apiKey=your-api-key-here`（将 `your-api-key-here` 替换为您的真实 API Key）

> **以账户页为准**：[且慢 MCP 账户页](https://qieman.com/mcp/account) 会展示与您账号对应的接入方式与完整 URL；**若页面与本文示例不一致，请以账户页为准。**

### 步骤 1：获取 API Key

1. 访问 [且慢 MCP 服务页面](https://qieman.com/mcp) 注册账号并了解服务
2. 登录后打开 [且慢 MCP 账户页](https://qieman.com/mcp/account)，申请并复制 MCP API Key
3. 妥善保存 API Key（后续配置时需要）

> 💡 **提示**：更多说明与 Key 管理以官网及账户页为准：[https://qieman.com/mcp](https://qieman.com/mcp)

### 步骤 2：在 Claude Desktop 中配置

Claude Desktop 仅支持本地 stdio 时，需使用 **Node.js / npm** 运行 `mcp-remote` 桥接远程服务。

#### 方式 A：SSE + mcp-remote（推荐，兼容性最好）

在 Claude Desktop 配置文件中添加：

```json
{
  "mcpServers": {
    "qieman": {
      "command": "npx",
      "args": [
        "-y",
        "mcp-remote",
        "https://stargate.yingmi.com/mcp/sse?apiKey=your-api-key-here"
      ]
    }
  }
}
```

**配置说明**：

- `mcp-remote`：将远程 MCP（SSE）桥接为本地 stdio，供 Claude Desktop 使用
- URL 中的 `your-api-key-here` 请替换为您的真实 API Key

#### 方式 B：Streamable HTTP + mcp-remote（可选）

若您使用的 `mcp-remote` 版本支持 Streamable HTTP，可使用 `**/mcp/v2`** 并通过请求头传递 API Key（与 Cursor 等方式一致）：

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
        "x-api-key:your-api-key-here",
        "--header",
        "Accept:application/json, text/event-stream"
      ]
    }
  }
}
```

> Windows 版 Claude Desktop 若在 `--header` 中带空格被错误拆分时，可将整段 header 写入环境变量并在 `args` 里引用（参见 `mcp-remote` 文档），或优先使用 **方式 A（SSE）**。若方式 B 出现 OAuth 发现、403 等与鉴权无关的报错，请改回方式 A 或升级 `mcp-remote` 后重试。

### 步骤 3：在其他 MCP 客户端中使用

#### Cursor IDE

**配置步骤**：

1. 打开 Cursor，进入**设置**
2. 打开 **MCP**
3. **添加 MCP Server**，按需填入下列之一并保存

**Streamable HTTP（推荐）**：

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

**SSE（备选）**：

```json
{
  "mcpServers": {
    "qieman": {
      "url": "https://stargate.yingmi.com/mcp/sse?apiKey=your-api-key-here"
    }
  }
}
```

**配置说明**：

- Streamable HTTP：将 `headers` 中的 `your-api-key-here` 替换为您的实际 API Key；`Accept` 建议保持与上例一致
- SSE：将 URL 中的 `your-api-key-here` 替换为您的实际 API Key
- 若 Cursor 提供传输类型选项，请选择 **Streamable HTTP**（或 HTTP）与 **SSE** 中与实际配置对应的一项
- Cursor 下载：[https://www.cursor.com/cn](https://www.cursor.com/cn)

#### Cherry Studio

**Streamable HTTP**：在连接类型中选择 **HTTP / Streamable HTTP**（名称以软件为准），服务器地址填 `https://stargate.yingmi.com/mcp/v2`，并在自定义请求头中设置 `**x-api-key`**（值为您的 API Key）及 `**Accept: application/json, text/event-stream`**（若软件支持填写 headers）。

**SSE**：

1. 打开 Cherry Studio
2. 连接类型选择：**sse**
3. 地址：

```
https://stargate.yingmi.com/mcp/sse?apiKey=your-api-key-here
```

**配置说明**：

- 将 `your-api-key-here` 替换为您的实际 API Key
- Cherry Studio 下载：[https://cherry-ai.com/](https://cherry-ai.com/)

**推荐配置**（可选）：

- 推荐模型：火山引擎 Deepseek-v3 模型
- 模型名称：`deepseek-v3-250324`

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

**SSE**：

```json
{
  "mcpServers": {
    "qieman": {
      "url": "https://stargate.yingmi.com/mcp/sse?apiKey=your-api-key-here"
    }
  }
}
```

> ⚠️ **兼容性说明**：不同客户端对 MCP 传输（Streamable HTTP / SSE）的支持不同；**请以客户端文档及 [且慢 MCP 账户页](https://qieman.com/mcp/account) 为准。**

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

- **云托管服务**：无需本地部署服务端代码，在客户端配置 **Streamable HTTP** 或 **SSE** 接入地址即可使用
- **专业可靠**：基于且慢投顾多年积累的金融数据与分析模型
- **实时更新**：支持实时获取最新基金净值、公告与市场资讯
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
- 官网地址: [https://qieman.com/mcp](https://qieman.com/mcp)

---

**由盈米且慢提供专业金融数据支持**