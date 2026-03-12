# PMM Partner

Your product marketing partner in Claude Code - GTM documentation, releases, ICPs, and competitive intel.

## What This Is

This plugin helps Product Marketing Managers (PMMs) use Claude Code to:
- Keep product documentation current
- Track releases and GTM activities
- Build and maintain GTM documentation
- Work directly inside Notion, Linear, and other tools

## Who This Is For

PMMs who:
- Want AI to work *inside* their tools, not in a separate chat window
- Are comfortable learning new things but aren't developers
- Need to maintain docs without relying on engineering

---

## Quick Start

### Step 1: Make sure you have Claude Code

Open your **Terminal** app (Cmd + Space, type "Terminal", press Enter) and type:

```
claude --version
```

If you see a version number, you're good! Skip to Step 2.

If you see "command not found", you need to install Claude Code first:
- [Getting Started Guide](guides/getting-started.md) - walks you through installation
- Or visit [Claude Code docs](https://docs.anthropic.com/en/docs/claude-code)

### Step 2: Download this plugin

**Option A: Download ZIP (easiest)**
1. Click the green **Code** button at the top of this page
2. Click **Download ZIP**
3. Unzip the file
4. Move the folder to your Desktop (or somewhere you can find it)

**Option B: Clone with git**
```
cd ~/.claude/plugins
git clone https://github.com/taylormichellejoyce-bit/pmm-partner.git pmm-partner
```

### Step 3: Install the plugin

Open **Terminal** and run the install script.

If you downloaded the ZIP to your Desktop:
```
cd ~/Desktop/pmm-partner-main
./install.sh
```

If you cloned with git:
```
cd ~/.claude/plugins/pmm-partner
./install.sh
```

The script will tell you if it worked!

### Step 4: Start using it

1. Open a **new** Terminal window
2. Type `claude` and press Enter
3. Once Claude Code starts, type: `/pmm-partner:setup`

The setup wizard will walk you through connecting your tools.

---

## What's the difference between Terminal and Claude Code?

This confuses everyone at first:

| Terminal | Claude Code |
|----------|-------------|
| The app where you type commands to your computer | Claude running inside Terminal |
| You're here when you see `yourname@computer ~ %` | You're here when you see the Claude prompt |
| Used for: installing things, navigating folders | Used for: talking to Claude, using plugins |

**To get into Claude Code:** Open Terminal, type `claude`, press Enter.

**To exit Claude Code:** Type `/exit` or press Ctrl+C.

---

## Manual Installation

If the install script doesn't work, run these commands in **Terminal** (not inside Claude Code):

```bash
# Create plugins folder if it doesn't exist
mkdir -p ~/.claude/plugins

# Navigate to where you downloaded the plugin and run:
claude plugins marketplace add /path/to/pmm-partner
claude plugins install pmm-partner@pmm-partner
```

Replace `/path/to/pmm-partner` with the actual path to the folder.

---

## Skills

### Getting Started

| Skill | What It Does |
|-------|--------------|
| `/pmm-partner:setup` | **Connect your tools.** Guided wizard to connect Claude Code to Notion, Linear, and other tools you use. Start here. |
| `/pmm-partner:brand` | **Set up your brand.** Define your voice, messaging pillars, colors, fonts, and terminology so everything Claude creates sounds and looks like your company. |

### Strategy & Planning

| Skill | What It Does |
|-------|--------------|
| `/pmm-partner:plan` | **Your GTM thought partner.** Think through releases, plan initiatives, connect dots across products, identify what documentation needs updating. Use this before jumping into asset creation. |

### Documentation

| Skill | What It Does |
|-------|--------------|
| `/pmm-partner:core-products` | **Document your products.** Create and maintain your Core Products database - the source of truth for what you sell, organized by capability. |
| `/pmm-partner:releases` | **Track what's shipping.** Log upcoming releases, track GTM readiness, generate enablement checklists, translate internal names to customer-facing messaging. |
| `/pmm-partner:icp` | **Build ICPs and personas.** Document your ideal customers - who they are, what they care about, how they buy. Go as deep as you need (quick profiles to full JTBD). |
| `/pmm-partner:competitive` | **Track competitors.** Document competitor positioning, build sales battlecards, analyze win/loss patterns, keep differentiation messaging current. |

### Asset Creation

| Skill | What It Does |
|-------|--------------|
| `/pmm-partner:assets` | **Create GTM deliverables.** Build one-pagers, slide decks, talk tracks, email campaigns. Pulls from your brand, products, and ICPs so assets come out aligned. Can generate HTML you deploy instantly or work with your existing templates. |

### Recommended Flow

```
setup → brand → plan → [documentation skills] → assets
```

1. **Setup** - Connect your tools
2. **Brand** - Define your voice and style
3. **Plan** - Think through what you're doing and why
4. **Document** - Build your foundation (products, releases, ICPs, competitive)
5. **Assets** - Create deliverables from your foundation

---

## Security

Before using PMM Partner, read the [Security & AI Usage Guidelines](SECURITY.md). Key points:
- Never put API keys, passwords, or customer data in AI prompts
- MCP connections grant real access - understand what you're connecting
- Always review before confirming destructive actions
- When in doubt, ask your Security/IT team

---

## Learn More

- [Start Here](guides/START_HERE.md) - What is Claude Code and why should you care?
- [Getting Started Guide](guides/getting-started.md) - Your first steps in the terminal
- [Framework Overview](frameworks/growthscript.md) - The framework explained
- [GTM Functions](frameworks/gtm-functions.md) - Key PMM activities and workflows

---

## Acknowledgments

This plugin was inspired by [PM Thought Partner](https://github.com/breethomas/pm-thought-partner) created by **Bree Thomas**. Her work showed what's possible when you bring product frameworks into Claude Code, and PMM Partner builds on that vision for the product marketing side.

---

## Questions?

This toolkit was created by Taylor Berry. Reach out at taylormichellejoyce@gmail.com
