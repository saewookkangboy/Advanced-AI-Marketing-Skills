---
title: MCP Marketing Data Integration
description: Connect Google Analytics, Search Console, and AdSense to your AI agent via MCP (Model Context Protocol).
---

# MCP Marketing Data Integration

This skill enables you to query real-time marketing data from Google Analytics, Search Console, and AdSense directly within your AI conversations using **Metrifyr** MCP Server.

## What is MCP?

**Model Context Protocol (MCP)** allows AI agents (like Claude) to connect to external data sources and tools. Instead of copy-pasting data, your AI can directly fetch live metrics.

## 🎯 Use Cases

- **Real-time Reporting**: "Show me yesterday's GA4 traffic by source."
- **SEO Analysis**: "What are my top 10 Search Console queries this week?"
- **Revenue Tracking**: "Compare AdSense revenue: this month vs last month."
- **Automated Insights**: "Analyze bounce rate trends and suggest improvements."

## 🚀 Setup Guide

### Option 1: Claude.ai (Web Interface)

1. **Go to Settings**:
    - Open [Claude.ai](https://claude.ai)
    - Click **Settings** → **Connectors**

2. **Add Metrifyr MCP Server**:
    - Click **Add custom connector**
    - Paste this URL:

    ```
    https://mcp.metrifyr.cloud/mcp
    ```

3. **Authenticate**:
    - Click **Connect your Google account**
    - Grant permissions for Analytics, Search Console, and AdSense

4. **Test Connection**:
    - Ask Claude: *"Show me my Google Analytics sessions from last 7 days."*

### Option 2: Claude Code / Desktop (CLI)

1. **Login to MCP**:

    ```bash
    npx mcp-google-marketing login
    ```

2. **Add to Claude Config**:

    ```bash
    claude mcp add google-marketing npx mcp-google-marketing
    ```

3. **Verify**:

    ```bash
    claude mcp list
    ```

## 📊 Example Queries

### Google Analytics 4

```
"What were my top 5 landing pages yesterday?"
"Show me user demographics breakdown for the last 30 days."
"Compare sessions: this week vs last week."
```

### Google Search Console

```
"What are my top 10 keywords by impressions this month?"
"Show me CTR trends for the last 3 months."
"Which pages have the lowest average position?"
```

### Google AdSense

```
"What's my AdSense revenue for today?"
"Compare earnings: this month vs last month."
"Show me top performing ad units."
```

## 🔗 Advanced: Combining with Other Skills

You can chain this skill with **Marketing Report Automator** for automated reporting:

**Step 1**: Fetch data via MCP

```
"Get GA4 sessions, bounce rate, and top sources for last 7 days."
```

**Step 2**: Generate report

```
"Use the marketing-report-automator skill to create a TYPE=WEEKLY report from this data."
```

## 📚 Resources

- **Metrifyr MCP Server**: [metrifyr.cloud](https://www.metrifyr.cloud)
- **Original GitHub Repo** (Deprecated): [freema/mcp-google-marketing](https://github.com/freema/mcp-google-marketing)
- **MCP Protocol Docs**: [modelcontextprotocol.io](https://modelcontextprotocol.io)

## ⚠️ Important Notes

- **Data Privacy**: Metrifyr is a third-party hosted service. Review their privacy policy before connecting.
- **Rate Limits**: Google APIs have rate limits. Avoid excessive queries.
- **Permissions**: Only grant the minimum required scopes (Analytics, Search Console, AdSense).

## 🛠️ Troubleshooting

**Issue**: "Connection failed"

- **Solution**: Re-authenticate your Google account in Metrifyr settings.

**Issue**: "No data returned"

- **Solution**: Ensure your Google Analytics property has data and the correct date range is specified.

**Issue**: "Permission denied"

- **Solution**: Check that you granted Analytics/Search Console/AdSense permissions during OAuth flow.
