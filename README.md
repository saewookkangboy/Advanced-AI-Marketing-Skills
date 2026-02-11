# Advanced AI Marketing Skills

Use these structured "Skills" to upgrade your AI agent (Claude Code, OpenClaw, Gemini) into a professional marketing team.

## 📦 Included Skills

### 1. 🎨 [Context Ad Generator](./context-ad-generator/SKILL.md)

**For**: Midjourney, Flux, DALL-E 3 users.
Creates high-end, art-directed image prompts by injecting photographer context (Camera, Lighting, Vibe).
**NEW Features**:

- 7 Styles: Cyberpunk, Neo-Noir, Cottagecore, Luxury, etc.
- Meta-Analysis step for better creative direction.

### 2. 🎬 [Viral Reels Scripter](./viral-reels-scripter/SKILL.md)

**For**: Social Media Managers, Content Creators.
Generates 15-60s video scripts optimized for retention.
**NEW Features**:

- Hook Frameworks: Negativity Bias, Curiosity Gap, Transformation.
- Niche-specific examples (Crypto, Productivity, etc.).

### 3. 📊 [One-Click Report Automator](./marketing-report-automator/SKILL.md)

**For**: Marketing Analysts, Agencies.
Instantly converts messy notes into professional reports.
**NEW Features**:

- Support for `TYPE=DAILY`, `TYPE=QBR` (Quarterly), and `TYPE=POST_MORTEM`.

### 4. 🔌 [MCP Marketing Data Integration](./mcp-marketing-data/SKILL.md)

**For**: Data-driven marketers using Claude.ai or Claude Code.
Connect Google Analytics, Search Console, and AdSense directly to your AI agent via MCP (Model Context Protocol).
**Features**:

- Real-time data queries (no copy-paste needed)
- Automated reporting from live sources
- Metrifyr MCP Server setup guide

## 🚀 How to Use

### Manual Usage

1. Navigate to the skill folder (e.g., `context-ad-generator`).
2. Copy the **Prompt Template** from `SKILL.md`.
3. Paste it into your AI chat (ChatGPT, Claude, Gemini) as a "System Prompt" or "Custom Instruction".

### Agent Usage (Claude Code / OpenClaw)

Copy the skills to your agent's skill directory:
\`\`\`bash
cp -r advanced-marketing-skills/* ~/.claude/skills/
\`\`\`
Then simply ask: *"Create a luxury ad prompt for my new watch."*

## 🤖 Virtual Product Team (Orchestration)

Build full software solutions by simulating a complete product team.

### 5. 👔 [Product Manager (Orchestrator)](./virtual-product-team/role-product-manager/SKILL.md)

**The Boss**. Starts here. Break down vague ideas into strict tasks for other roles.
*Usage*: "Act as PM. Plan a new referral system."

### 6. 🎨 [UI/UX Designer](./virtual-product-team/role-ui-ux-designer/SKILL.md)

**The Architect**. Creates wireframes and design systems (Tailwind).

### 7. 💻 [Frontend Developer](./virtual-product-team/role-frontend-dev/SKILL.md)

**The Builder**. Writes React/Vue components based on the design.

### 8. ⚙️ [Backend Developer](./virtual-product-team/role-backend-dev/SKILL.md)

**The Logic**. Builds APIs and business logic.

### 9. 🛡️ [Security Engineer](./virtual-product-team/role-security-engineer/SKILL.md) & 🗄️ [Database Admin](./virtual-product-team/role-database-admin/SKILL.md)

**The Guardians**. Ensure safety and data integrity.

### 🔄 Valid Orchestration Workflow

1. **User** → **PM**: "I want a dashboard."
    - *Result*: PRD with tasks for functional roles.
2. **User** → **Designer**: "Generate wireframes for task 1 from PRD."
3. **User** → **Frontend**: "Implement the wireframe."
4. **User** → **Backend**: "Build the API for this component."
5. **User** → **Security**: "Audit the code."

## 💾 Token Optimization (Global System Prompt)

To maximize cost-efficiency across all skills, append this instruction to your custom instructions:

```text
[Global Protocol]
1. NO YAPPING: Do not output conversational filler ("Here is the code", "Sure", "I hope this helps").
2. CODE ONLY: When asked for code, output ONLY the code block.
3. EXCEPTION REPORTING: When analyzing data, only output significant anomalies (>10% variance).
4. CONCISE FORMAT: Use tables and bullet points. Avoid paragraphs.
```

## 📚 References & Resources

### Reference

- **[BrianRWagner/ai-marketing-skills](https://github.com/BrianRWagner/ai-marketing-skills)**: Please refer to this repository for basic marketing skill features!

### External Tools

For additional content creation prompts, visit **[prompt.allrounder.im](https://prompt.allrounder.im/)**:

- Blog Content Generation
- Image Generation
- Video Generation
- ➕ And other useful prompts


## ✍️ Credits

This entire repository was written by **Google Antigravity**.

Made with Chunghyo, Ideation with Chunghyo (email chunghyo@troe.kr)
