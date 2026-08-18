# Yingmi Investment Advisory MCP Server

Yingmi Investment Advisory MCP Server is an intelligent investment advisory service based on the Model Context Protocol (MCP), providing AI assistants with professional fund analysis, asset allocation, and portfolio diagnostics capabilities. Make investment decisions smarter and more efficient through natural language interaction. Register, product information, and the open platform home are on the **[Yingmi AI Open Platform](https://ai.yingmi.com)**; API keys and endpoint details follow what you see in the platform console.

## Core Capabilities

### 📊 Personal & Household Finance Analysis

- **Asset-Liability Analysis**: Intelligent calculation of asset-liability ratios, net worth, and core financial metrics
- **Cash Flow Analysis**: Generate cash flow health reports based on household income/expenses and asset allocation
- **Family Member Analysis**: Statistics on family size and life cycle stages with customized recommendations
- **Financial Indicator Diagnostics**: Assess the rationality of key financial indicators and identify potential risks
- **Income-Expense Structure Analysis**: Visualize annual income/expense distribution and optimize financial planning

### 💼 Fund & Portfolio Analysis

- **Fund Risk Assessment**: Multi-dimensional risk scoring and indicator analysis (volatility, max drawdown, Sharpe ratio, etc.)
- **Portfolio Risk Diagnostics**: Overall portfolio risk assessment and optimization recommendations
- **Holdings Diagnostics**: In-depth analysis of fund allocation rationality, correlation, and historical backtesting performance
- **Asset Allocation Analysis**: Fund portfolio asset class penetration to identify hidden risks
- **Correlation Analysis**: Discover correlations between funds to avoid over-concentration
- **Backtesting Simulation**: Historical backtesting and Monte Carlo simulation to estimate potential return and risk ranges under different scenarios

### 🔍 Fund Information Query

- **Fund Details**: Batch retrieval of comprehensive fund information including NAV, performance, fees, and trading rules
- **Performance Diagnostics**: Valuation level and performance attribution analysis
- **Smart Search**: Support fuzzy matching of fund names and multi-dimensional filtering and sorting
- **Popular Funds**: Retrieve recently popular funds and market attention trends
- **Trading Rule Query**: Timely access to fund trading rules and subscription/redemption limits

### 📈 Professional Investment Analysis

- **Industry Allocation Analysis**: Fund industry preferences, concentration, and revenue contribution analysis
- **Bond Indicators**: Professional bond fund indicators including duration, leverage, and credit ratings
- **Equity Indicators**: Equity position, turnover rate, market timing ability, and Brinson attribution analysis
- **QDII Analysis**: Overseas fund regional allocation and risk assessment
- **Strategy Research**: Fund strategy details, risk information, and asset penetration

### 🛠️ Auxiliary Tools

- **Data Visualization**: ECharts chart rendering for intuitive display of analysis results
- **Report Generation**: HTML to PDF conversion for professional investment reports
- **Real-time News**: Financial news, hot topics, and fund manager viewpoint search
- **AI Interpretation**: Real-time AI news interpretation and investment advisory content recommendations

## Use Cases

### Individual Investors

- Quickly diagnose risk and return characteristics of existing fund portfolios
- Obtain professional asset allocation recommendations and optimization solutions
- Track market hotspots and latest fund manager viewpoints

### Investment Advisors

- Provide clients with professional financial planning and asset allocation services
- Batch analyze fund products and quickly generate investment reports
- Query and assess portfolio risks to inform investment-strategy adjustments

### Financial Researchers

- In-depth analysis of fund performance attribution and risk sources
- Research industry allocation trends and market rotation patterns
- Backtest investment strategies and validate investment logic

## Complete Tool List (69)

### Financial Data (35)

#### Fund Data (28)

- SearchFunds - Search Funds
- BatchGetFundNavHistory - Fund NAV History
- BatchGetFundsDetail - Batch Get Fund Details
- GetBatchFundPerformance - Batch Get Fund Performance
- AnalyzeFundRisk - Fund Risk Analysis
- BatchGetFundTradeLimit - Fund Trading Limits
- BatchGetFundsDividendRecord - Fund Dividend Records
- fund-equity-position - Equity Position Preference
- getFundIndustryAllocation - Industry Allocation Weights
- BatchGetFundTradeRules - Fund Trading Rules
- getFundTurnoverRate - Fund Turnover Rate (Rebalancing Frequency)
- getFundBenchmarkInfo - Fund Performance Benchmark
- getStockAllocationAndMetricsByFundCode - Valuation Metrics (PE / PB / ROE)
- getFundBrinsonIndicator - Brinson Attribution
- GetFundAssetClassAnalysis - Asset-Class Distribution
- getBondIndicator - Bond Fund Risk
- fund-recovery-ability - Drawdown Recovery Ability
- getFundIndustryConcentration - Industry Concentration
- getFundIndustryReturns - Industry Return Contribution
- getFundCampisiIndicator - Campisi Attribution
- getBondAllocationByFundCode - Bond-Type Allocation
- getFundIndustryPreference - Fund Industry Preference
- fund-sector-preference - Fund Sector Preference
- getQdFundAreaAllocation - QDII Regional Allocation
- getMarketTimingIndicator - Equity Market Timing
- BatchGetFundsSplitHistory - Fund Split Records
- getFundDiveCount - Bond Fund Abnormal Moves
- getBondFundCreditRatingLevel - Bond Fund Credit-Rating Breakdown

#### Strategy Data (7)

- GetStrategyDetails - Strategy Details
- GetStrategyAssetClassAnalysis - Strategy Asset-Class Distribution
- BatchGetStrategiesComposition - Batch Query Strategy Holdings
- GetStrategyRiskInfo - Strategy Risk
- GetStrategyBenchmark - Strategy Performance Benchmark
- GetPortfolioNavHistory - Portfolio NAV History
- BatchGetPoTradeComposition - Strategy Trade Composition

### Investment Research (13)

#### Pre-investment Analysis (8)

- GetFundDiagnosis - Fund Diagnosis
- GetPopularFund - Recent Popular Funds
- GetLatestQuotations - Market Thermometer
- GetFundRelatedStrategies - Filter Advisory Strategies by Overweight Fund
- getBondFundWithAlertRecord - Bond Funds with NAV Alerts
- filterBondFundByBondType - Filter Funds by Bond-Type Style
- filterBondFundByCreditRating - Filter Funds by Credit Rating
- filterStockFundByStockTurnover - Filter Funds by Stock Turnover

#### Calculation (2)

- GetFundsBackTest - Backtest Analysis
- MonteCarloSimulate - Portfolio Expected-Return Simulation (Monte Carlo)

#### Post-investment Diagnosis (3)

- AnalyzePortfolioRisk - Post-investment Risk Analysis
- GetFundsCorrelation - Fund Correlation Analysis
- GetAssetAllocation - Asset Allocation Analysis

### General Services (5)

#### Financial Tools (1)

- GuessFundCode - Fuzzy Fund-Code Matching

#### Common Tools (4)

- GetCurrentTime - Get Current Time
- RenderEchart - ECharts Chart Rendering
- RenderHtmlToPdf - HTML to PDF
- GetTxnDayRange - Trading-Day Query

### Investment Advisory Services (11)

#### Investment Advisor (11)

- GetAssetAllocationPlan - Get Asset Allocation Plan
- StrategySearchByKeyword - Strategy Keyword Search
- AnalyzeFinancialIndicators - Financial Condition Analysis
- DiagnoseFundPortfolio - Account Diagnosis
- GetCompositeModel - Get Fund Investment Plan
- BatchGetStrategyRiskInfo - Strategy Risk Matching
- AnalyzeInvestmentPerformance - Investment Plan Performance Analysis
- AnalyzeFamilyMembers - Household Structure Analysis
- AnalyzeCashFlow - Cash Flow Analysis and Financial Planning
- AnalyzeAssetLiability - Asset-Liability Analysis
- AnalyzeIncomeExpense - Income and Expense Analysis

### Investment Advisory Content (5)

#### Public Content (2)

- SearchFinancialNews - Financial News
- SearchHotTopic - Hot Financial Topics

#### Yingmi Original Content (3)

- SearchManagerViewpoint - Fund Manager Viewpoints
- searchInvestAdvisorContent - Search Advisory Content
- searchRealtimeAiAnalysis - Real-time News AI Interpretation

## Quick Start

### Access Method: Cloud Hosted (Streamable HTTP)

Yingmi Investment Advisory MCP Server uses a **cloud-hosted model**. No local server deployment is required. Connect using **Streamable HTTP** (the recommended HTTP transport in current MCP specs; exact labels may vary by client).

**Endpoint**: `https://stargate.yingmi.com/mcp/v2` — authenticate with the **`x-api-key`** request header; set **`Accept`** to **`application/json, text/event-stream`**

> **Source of truth**: The [Yingmi AI Open Platform — Personal Center](https://ai.yingmi.com/mcp/account) shows the exact URLs and options for your account. **If anything differs from this document, follow the platform console.**

### Step 1: Get API Key

1. Open the [Yingmi AI Open Platform](https://ai.yingmi.com) to sign up and learn about the product
2. Sign in and go to the [Yingmi AI Open Platform — Personal Center](https://ai.yingmi.com/mcp/account) to create or copy your MCP API Key
3. Store your API Key securely (you will need it in the next steps)

> 💡 **Tip**: For the latest guidance and key management, see the [Yingmi AI Open Platform](https://ai.yingmi.com) and the [Yingmi AI Open Platform — Personal Center](https://ai.yingmi.com/mcp/account).

### Step 2: Configure in Claude Code

Claude Code supports remote HTTP MCP servers natively, so `mcp-remote` is not required. The recommended setup is a `.mcp.json` file in the project root with the API Key supplied through an environment variable:

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

Set the `YINGMI_API_KEY` environment variable before use, then restart Claude Code. You can also add the server directly from the CLI:

```powershell
claude mcp add --transport http --scope user qieman https://stargate.yingmi.com/mcp/v2 --header "x-api-key: your-api-key-here" --header "Accept: application/json, text/event-stream"
```

> The CLI form writes the request headers to the Claude Code configuration. Use the `.mcp.json` + environment-variable form above if you do not want the Key stored in plaintext. Run `claude mcp list`, or enter `/mcp` in Claude Code, to verify the connection.

### Step 3: Configure in Claude Desktop

Claude Desktop **Connectors** are intended for remote MCP servers that support OAuth or require no authentication. The current Yingmi MCP endpoint requires a custom `x-api-key` header, so it cannot be connected by entering only its URL in Connectors. Use `mcp-remote` as a local stdio compatibility bridge. If the Yingmi AI Open Platform later provides an OAuth-compatible Connector URL, follow the console guidance and add it through **Settings → Connectors → Add custom connector** instead.

#### Claude Desktop + mcp-remote (compatibility option)

Add the following to your Claude Desktop configuration file (Node.js is required, and your `mcp-remote` version must support Streamable HTTP):

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

**Configuration notes**:

- This registers a local stdio bridge process; it does not register a remote HTTP server directly in `claude_desktop_config.json`
- `mcp-remote` bridges the remote Streamable HTTP MCP server to local stdio for Claude Desktop
- Replace `your-api-key-here` in `env.YINGMI_API_KEY` with your real API Key
- On Windows, the header arguments contain no spaces; complete values containing spaces are injected through `env` so Claude Desktop does not split them when invoking `npx`
- This compatibility setup stores the Key in the local Claude Desktop configuration file. Do not commit that file to Git, and restrict access to it

> Restart Claude Desktop after saving. If the connection fails, verify the API Key and endpoint first, then upgrade `mcp-remote` and inspect the Claude Desktop MCP logs.

### Step 4: Use in Other MCP Clients

#### Cursor IDE

**Steps**:

1. Open Cursor **Settings**
2. Open **MCP**
3. **Add MCP Server** and paste the following

**Streamable HTTP**:

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

**Notes**:

- Put your real API Key in `headers.x-api-key`; keep `Accept` as shown
- If Cursor asks for a transport type, choose **Streamable HTTP** (or HTTP) to match this config
- Cursor download: [https://www.cursor.com/cn](https://www.cursor.com/cn)

#### Codex (CLI / IDE)

Codex CLI and the IDE extension read remote MCP servers from `~/.codex/config.toml` (on Windows: `%USERPROFILE%\.codex\config.toml`). ChatGPT on the web does not read this local configuration.

```toml
[mcp_servers.qieman]
url = "https://stargate.yingmi.com/mcp/v2"
env_http_headers = { "x-api-key" = "YINGMI_API_KEY" }
http_headers = { "Accept" = "application/json, text/event-stream" }
```

**Notes**:

- Set the `YINGMI_API_KEY` environment variable before use, then restart Codex
- The `env_http_headers` value is the environment-variable name, not the API Key itself; do not also put a plaintext `x-api-key` in `http_headers`
- Config reference: [Codex config.toml](https://learn.chatgpt.com/docs/config-file/config-reference)
- You can also run `codex mcp add qieman --url https://stargate.yingmi.com/mcp/v2`, then add the headers above to `config.toml`

#### Cherry Studio

Choose **HTTP** or **Streamable HTTP** (label varies). Set the server URL to `https://stargate.yingmi.com/mcp/v2` and add custom headers **`x-api-key`** (your API Key) and **`Accept: application/json, text/event-stream`** if the app supports headers.

**Notes**:

- Cherry Studio download: [https://www.cherryai.com.cn/](https://www.cherryai.com.cn/)

#### Windsurf / Trae / Other IDEs

**Streamable HTTP** (same shape as Cursor when `headers` are supported):

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

> ⚠️ **Compatibility**: Client support for **Streamable HTTP** may vary. **Follow your client’s documentation and the [Yingmi AI Open Platform](https://ai.yingmi.com) console.**

### Usage Examples

**Scenario 1: Diagnose Fund Portfolio**

```
I hold the following funds: E Fund Blue Chip Select (005827), Xingquan Heren (163406), China Europe Pioneer (001938). Please analyze the portfolio's risk and correlation.
```

**Scenario 2: Asset Allocation Recommendation**

```
I have 1 million yuan in capital with moderate risk tolerance and expect an annualized return of around 8%. Please design an asset allocation plan for me.
```

**Scenario 3: Performance Attribution Analysis**

```
Using the Campisi model, break down the total return of Huaxia Bond Fund Class A (fund code: 001001) from June 30 to September 30, 2025. What are the contribution ratios of interest rate changes, credit spread movements, coupon income, and other factors?
```

## Technical Features

- **Cloud Hosted**: No local server deployment required; connect using a **Streamable HTTP** endpoint URL in your client
- **Professional & Reliable**: Based on Yingmi Investment Advisory’s years of accumulated financial data and analytical models
- **Data Updates**: Retrieve the latest fund NAV and market news
- **Intelligent Analysis**: Combined with AI capabilities for natural language interactive investment analysis
- **Visualization**: Built-in chart rendering and report generation for clear results
- **Standard Protocol**: Based on MCP protocol, compatible with Claude Desktop, Cursor, Trae and other mainstream AI tools
- **Secure & Controlled**: API Key authentication, encrypted data transmission for information security

## Disclaimer

All information, analysis, and recommendations provided by this service are for reference only and do not constitute any investment advice or guarantee. Investment involves risks, and decisions should be made with caution. The developers and service providers are not responsible for any investment losses resulting from the use of this service. Please make investment decisions based on your own circumstances with a full understanding of the risks.

## License

MIT License

## Contact

- Feedback: [wangjiaye@yingmi.cn](mailto:wangjiaye@yingmi.cn)
- GitHub: [Yingmi-MCP](https://github.com/yingmi-dev/Yingmi-MCP)
- Open platform: [Yingmi AI Open Platform](https://ai.yingmi.com)

---

**Powered by Yingmi Investment Advisory with Professional Financial Data Support**
