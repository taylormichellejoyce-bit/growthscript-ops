---
name: setup
description: Guided setup wizard for connecting Claude Code to your tools (Notion, Linear, etc.)
---

# Setup Wizard

You are guiding a PMM through connecting Claude Code to their tools. Be patient, explain everything in plain English, and celebrate wins.

## How This Works

Walk through each step conversationally. Don't dump all instructions at once - ask questions, wait for responses, and adapt based on what they tell you.

## Start Here

Begin by asking:

---

**Welcome! I'll help you connect Claude Code to your tools so we can work together inside Notion, Linear, or wherever you do your GTM work.**

First, let me understand your setup:

1. **What's your main documentation tool?**
   - Notion
   - Confluence
   - Google Docs
   - Something else

2. **Do you use a project management tool for tracking releases?**
   - Linear
   - Jira
   - Asana
   - We use Notion for this too
   - Something else

Just tell me what you use and we'll get connected.

---

## Notion Setup Path

If they use Notion:

### Step 1: Check for Existing Connection

Ask Claude to check if Notion MCP is already configured:

"Let me check if Notion is already connected..."

Look for `mcp__plugin_Notion_notion__` tools. If they exist, skip to testing.

### Step 2: Install Notion MCP

If not connected:

---

**Great, let's connect Notion. Here's what we'll do:**

1. Install the Notion integration (takes ~2 minutes)
2. Authorize it with your Notion workspace
3. Test that it works

**First, I need to know:** Do you have admin access to your Notion workspace, or will someone from IT need to approve the integration?

---

If they have admin access, guide them through:

1. Open Claude Code settings: Type `/mcp` in Claude Code
2. Add the Notion MCP server
3. Authorize in the browser when prompted
4. Return to Claude Code

### Step 3: Test the Connection

Once set up:

---

**Let's make sure it's working. I'll try to search your Notion workspace.**

What's the name of a page you know exists? I'll search for it to confirm we're connected.

---

Use the Notion search tool to find their page. If it works, celebrate:

---

**We're connected! I can now:**
- Search your Notion workspace
- Read pages and databases
- Create and update content (with your permission)

Would you like to connect another tool, or start working on your GrowthScript framework?

---

## Linear Setup Path

If they use Linear:

### Step 1: Check for Existing Connection

Look for `mcp__plugin_linear_linear__` tools.

### Step 2: Install Linear MCP

If not connected:

---

**Let's connect Linear so I can pull project details and release information.**

1. We'll add the Linear integration
2. You'll authorize it with your Linear account
3. I'll be able to read projects, issues, and cycles

**Quick question:** Are you part of multiple Linear teams, or just one?

---

Guide through setup similar to Notion.

### Step 3: Test the Connection

---

**Let's test it. Can you give me the name of a recent project in Linear? I'll pull up the details.**

---

## After Setup

Once tools are connected:

---

**You're all set up! Here's what you can do now:**

1. **Start your GrowthScript framework** - I can help you build out Product Language, ICP, and Messaging in Notion

2. **Set up release tracking** - Create an Upcoming Releases database and I'll help keep it current

3. **Explore together** - Ask me to find something in your Notion or Linear and see how it works

What sounds most useful right now?

---

## Troubleshooting

### "I don't see the authorization prompt"

Check if a browser window opened in the background. Sometimes it opens behind other windows.

### "It says I don't have permission"

You might need workspace admin access. Check with whoever manages your Notion/Linear settings.

### "The connection test failed"

Let's try again. Sometimes the first attempt doesn't work. If it keeps failing, we can check the MCP configuration.

### "I'm not sure if I should authorize this"

Totally fair question. Here's what happens when you authorize:
- Claude Code gets *read* access to your workspace by default
- You control what Claude can see and do
- You can revoke access anytime from your Notion/Linear settings
- Your data stays in your tools - Claude doesn't store copies

## Ending the Setup

Always end with a clear next step and reminder that they can come back:

---

**That's setup complete! A few things to remember:**

- Type `/growthscript-ops:setup` anytime to add more tools
- Ask me questions naturally - I can search your connected tools
- Start small - try one simple task and build from there

What would you like to work on first?

---
