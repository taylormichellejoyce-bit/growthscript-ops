# Getting Started with Claude Code

A friendly guide for PMMs who've never used a terminal before.

---

## What Is Claude Code?

Claude Code is Claude (the AI) running in your terminal instead of a chat window. The difference?

| ChatGPT/Claude.ai | Claude Code |
|-------------------|-------------|
| You copy context in, copy output out | Claude reads your files and tools directly |
| Generates text for you to paste | Takes action inside your tools |
| You are the middleware | Claude is your partner |

**The big idea:** Instead of copying information between ChatGPT and Notion, Claude Code works *inside* Notion directly.

---

## Before You Start

You'll need:
- [ ] A Mac (this guide is Mac-focused; Windows/Linux work too but steps differ)
- [ ] An Anthropic account with Claude Code access
- [ ] About 30 minutes for initial setup

---

## Step 1: Meet Your Terminal

The terminal is a text-based app where you type commands. It's already on your Mac.

**To open it:**
1. Press `Cmd + Space` (opens Spotlight search)
2. Type `Terminal`
3. Press Enter

You'll see a window with some text and a blinking cursor. That's it - you're in the terminal.

**What you're looking at:**
```
taylor@Taylors-MacBook ~ %
```
- `taylor` = your username
- `Taylors-MacBook` = your computer name
- `~` = you're in your home folder
- `%` = the terminal is ready for you to type

**Try it:** Type `pwd` and press Enter. This shows your current location (folder path).

### Make Your Terminal Friendlier (Optional)

The default Mac terminal works fine, but there are tools that make Claude Code easier to use — especially for managing multiple conversations.

**[cmux](https://www.cmux.dev/)** is built specifically for Claude Code. It gives you:
- A sidebar showing your conversation history
- Easy switching between sessions
- A cleaner interface than the raw terminal

**Other options:**
- **[Warp](https://www.warp.dev/)** — Modern terminal with AI features and a more visual interface
- **[iTerm2](https://iterm2.com/)** — Popular Mac terminal with split panes and customization
- **tmux** — For power users who want full control over terminal sessions

You don't need any of these to get started — the default terminal works. But if the raw terminal feels overwhelming, these tools can help.

**The bigger point:** Claude can help you customize your setup. Ask things like "What's the best terminal app for someone new to the command line?" or "Help me configure cmux." Claude isn't just for PMM work — it's a partner for figuring out whatever you need.

---

## Step 2: Install Claude Code

There are a few ways to install Claude Code. Pick whichever works for you:

**Option A: Direct download (recommended for beginners)**

Visit the [Claude Code installation page](https://docs.anthropic.com/en/docs/claude-code) and follow their instructions.

**Option B: Using Homebrew (if you have it)**

```bash
brew install claude-code
```

**Option C: Using npm (if you have Node.js)**

```bash
npm install -g @anthropic-ai/claude-code
```

**How do I know if it worked?**

Type this and press Enter:
```bash
claude --version
```

If you see a version number, you're good!

---

## Step 3: Log In

Type this and press Enter:

```bash
claude
```

The first time you run this, it will:
1. Open your browser to log in with your Anthropic account
2. Ask you to authorize Claude Code
3. Return you to the terminal, now logged in

**You'll know it worked when you see:** A welcome message and a prompt waiting for your input.

---

## Step 4: Your First Conversation

Now you're talking to Claude in your terminal. Try typing:

```
What can you help me with?
```

Claude will respond right there in the terminal. You can have a normal conversation, just like in Claude.ai.

**To exit:** Type `/exit` or press `Ctrl + C`

---

## Step 5: Understanding What Claude Can Do

In Claude Code, Claude can:

| Action | What It Means |
|--------|---------------|
| **Read files** | Look at documents on your computer |
| **Edit files** | Make changes to documents (with your permission) |
| **Run commands** | Execute terminal commands (with your permission) |
| **Connect to tools** | Work inside Notion, Linear, Slack via MCP |

**Important:** Claude always asks permission before making changes. You stay in control.

---

## The Permission System

When Claude wants to do something, you'll see a prompt like:

```
Claude wants to: Edit file ~/Documents/release-notes.md
Allow? [y/n/always]
```

Your options:
- `y` = Yes, do it this once
- `n` = No, don't do it
- `always` = Yes, and don't ask again for this type of action

**Start with `y`** until you're comfortable. You can always say no.

---

## What's Happening When Claude "Works"

When Claude is doing something, you might see:
- Thinking indicators (dots or spinner)
- Tool calls (Claude is reading a file, searching, etc.)
- Output appearing line by line

**This is normal.** Claude is:
1. Thinking about your request
2. Deciding what tools to use
3. Taking action (with your permission)
4. Showing you the results

If something seems stuck, you can press `Ctrl + C` to stop it.

---

## Common Fears (and Why They're Okay)

**"What if I break something?"**
Claude asks permission before changing anything. If you're unsure, say no. You can also work in a test folder first.

**"What if Claude sees sensitive data?"**
Claude only sees what you give it access to. When connecting tools like Notion, you control which workspaces and pages are shared.

**"What if I type the wrong command?"**
The terminal will just say "command not found" - nothing breaks. And Claude explains commands before running them.

**"This looks like hacking."**
It's not! The terminal is just another way to use your computer. Developers use it daily. Now you can too.

---

## Next Steps

Now that you're set up:

1. **Connect your tools** - Run `/setup` in Claude Code for a guided walkthrough
2. **Learn GrowthScript** - Read the [GrowthScript Framework](../frameworks/growthscript.md)
3. **Start small** - Ask Claude to help you with one simple task first

---

## Quick Reference

| Command | What It Does |
|---------|--------------|
| `claude` | Start Claude Code |
| `/exit` | Leave Claude Code |
| `/help` | See available commands |
| `/setup` | Guided tool setup (this plugin) |
| `Ctrl + C` | Stop whatever's running |
| `pwd` | Show current folder |
| `ls` | List files in current folder |
| `cd ~/Documents` | Go to Documents folder |

---

## Need Help?

- Type `/help` in Claude Code for command reference
- Ask Claude directly - "I'm confused about X, can you explain?"
- Reach out to taylormichellejoyce@gmail.com

Remember: Everyone starts somewhere. The terminal feels foreign at first, but you'll get comfortable quickly.
