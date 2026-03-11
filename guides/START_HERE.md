# Start Here: What is Claude Code?

Before you dive into setup guides and workflows, let's answer the question you're probably asking: **What is this thing, and why should I care?**

---

## The Short Version

Claude Code is Claude running in your terminal. Instead of chatting in a browser window, Claude can actually *see* your files, *browse* your folders, and *take action* on your computer.

That's the technical description. Here's what it means for you:

**You stop being the middleware.**

No more copying context into ChatGPT, copying outputs back out, pasting into Notion, updating your docs manually, and repeating this forever. Claude Code works *inside* your tools. It reads from your sources, writes to your destinations, and remembers what you've told it.

---

## How Claude Code is Different

You might already use Claude in other ways. Here's how they compare:

| Product | What It Is | Best For |
|---------|-----------|----------|
| **Claude.ai** | Web chat interface | Quick questions, one-off tasks |
| **Claude Projects** | Web chat + uploaded files | Ongoing conversations with context |
| **Claude Desktop** | Mac/Windows app | Same as web, native experience |
| **Claude Code** | Claude in your terminal | Building systems, taking action, working across tools |

The key difference: **Claude Code can act, not just chat.**

- It can read files on your computer
- It can write and edit files
- It can run commands
- It can connect to your tools (Notion, Linear, Slack, etc.)
- It remembers instructions across sessions

---

## Why This Matters for PMMs

### Stop Repeating Yourself

Every time you open ChatGPT, you start from zero. You paste in context. You explain who you are. You remind it of your products, your personas, your messaging.

With Claude Code, you set up your context *once*. Your GrowthScript framework, your product language, your company's way of doing things — Claude remembers it all.

### Build Systems That Compound

Instead of one-off outputs, you build workflows that get better over time. Update your messaging pillars in Notion, and Claude uses the updated version automatically. Add a new product to your docs, and it's available everywhere Claude works.

### Work in Parallel

Claude Code can run tasks while you do other work. Start a research task, switch to something else, come back to the results. You're not waiting on a chat window.

### Own Your Data

Everything runs locally on your machine. Your files stay your files. Claude connects to your tools through official integrations, not by you pasting sensitive data into a browser.

---

## "But I'm Not Technical..."

This is the most common objection. Let's address it directly.

**You don't need to be a developer to use Claude Code.**

Yes, it runs in the terminal. Yes, that sounds technical. But here's the reality:

- The terminal is just a text-based way to talk to your computer
- You type commands, you see results
- Claude Code does most of the technical work for you
- You're mostly typing in plain English and letting Claude figure out the details

If you can write an email, you can use Claude Code. The learning curve is real but short. Most people get comfortable within a few sessions.

**What you DO need:**
- Willingness to try something new
- Patience for a few "wait, what just happened?" moments
- About 30 minutes to get set up

**What you DON'T need:**
- Programming knowledge
- GitHub experience
- Command line expertise
- A computer science degree

---

## The Mindset Shift

Using Claude Code requires a small but important shift in how you think about AI tools:

**Old way:** AI is a chat window. You ask, it answers, you copy, you paste.

**New way:** AI is an assistant with hands. You give it access to your work, and it helps you *do things*, not just *talk about things*.

This is the difference between asking someone for directions versus having them drive you there.

---

*The sections below are adapted from Teresa Torres' [Claude Code Recipes](https://www.producttalk.org/) series on Product Talk. Her practical, non-technical approach to Claude Code inspired much of this guide.*

---

## How Claude Remembers Things

With ChatGPT or Claude.ai, every conversation starts from scratch. You paste in context, explain who you are, remind it of your products. Every. Single. Time.

Claude Code is different. You can give it a **memory** — files that persist across sessions and tell Claude what it needs to know about you and your work.

### The Three-Layer Memory System

Think of it like layers of context that stack on top of each other:

| Layer | What It Is | When It Loads |
|-------|-----------|---------------|
| **Global** | How you like to work (preferences, style, communication) | Every session, everywhere |
| **Project** | Rules for this specific work (this product, this team) | When you're in that folder |
| **Reference** | Detailed context (products, personas, competitors) | Only when Claude needs it |

**Why layers matter:**

- **Global preferences** mean you don't repeat yourself. "Always ask before making changes" or "Give me direct feedback" — set it once, done forever.
- **Project instructions** let different work have different rules. Your GrowthScript work is different from your weekly reporting.
- **Reference files** give Claude deep context without overloading it. When you ask for help with a landing page, Claude pulls in your product file and target audience — not everything you've ever told it.

### What to Put in Memory (For PMMs)

The most valuable context files for product marketing:

- **Products and services** — What you sell, features, capabilities, packaging
- **Target customers** — ICP details, personas, what they care about
- **Competitors** — Who else is in the space, how you're different
- **Writing style** — Your brand voice, terminology, what to avoid

You don't have to create all of this at once. Build it iteratively:
- When you catch yourself explaining the same thing twice, create a file for it
- When Claude gives you generic output, add more context
- At the end of work sessions, ask: "What should we save for next time?"

### The Payoff

Once your memory is set up, your prompts become simple:

> "Help me write a one-pager for the new reporting feature"

Claude already knows your products, your personas, your voice. You don't have to explain. It just works.

---

## Building Workflows

The real power of Claude Code isn't one-off tasks — it's building workflows that you can reuse.

### Start by Mapping What You Do

Before you automate anything, write down every step of how you complete a task manually. For example, when you update product docs after a release:

1. Check Linear for what shipped
2. Read the spec/PRD
3. Find existing docs that need updates
4. Draft the changes
5. Get review
6. Publish

This is like story mapping, but for your own process. Once you see the steps, you can ask: "Where can Claude help?"

### Choose One Step (Not All of Them)

Don't try to automate everything at once. Pick one step — ideally something tedious or that you don't enjoy.

**Automate vs. Augment:**
- **Automate** = Claude does it for you (you review the output)
- **Augment** = Claude helps you do it better (you're still driving)

Most PMM work is augmentation. Claude helps you draft, research, and organize — but you make the final calls on messaging and positioning.

### Know What's Good for AI

Not everything benefits equally from AI assistance:

| Good for AI | Keep Doing Yourself |
|-------------|---------------------|
| Summarizing long documents | Final messaging decisions |
| Generating draft options | Brand voice judgment calls |
| Research and competitive analysis | Stakeholder relationships |
| Formatting and organizing | Strategic prioritization |
| Finding patterns in data | Knowing what matters to your customers |

### Save Repeatable Workflows as Commands

When you find yourself asking Claude to do the same thing repeatedly, save it as a slash command. A slash command is a shortcut — you type `/headlines` and Claude knows exactly what to do.

What goes in a command:
1. **What context Claude needs** — which files to read, what to know
2. **What process to follow** — step by step instructions
3. **How to format output** — where to save it, what structure to use
4. **Your preferences** — things like "no clickbait" or "match our brand voice"

You don't have to write these from scratch. Tell Claude: "Let's create a slash command that generates release notes from Linear specs" and work together to build it.

### Test and Iterate

Your first version won't be perfect. Use it a few times, notice what's wrong, and ask Claude to help you fix it.

> "The headlines you're generating are too long. Can we update the command to cap them at 10 words?"

This is normal. Workflows get better over time as you refine them.

---

## Choosing What to Automate

Not everything is worth automating. Here's how to decide where to focus.

### Three Goals for AI Assistance

1. **Do more of what you're good at** — Use AI to augment your strengths, not replace them
2. **Eliminate friction in frequent tasks** — Automate the tedious parts of things you do often
3. **Remove what drains you** — Hand off tasks you'd delegate if you could

### Seven Questions to Evaluate a Task

Before building a workflow, ask yourself:

| Question | What It Tells You |
|----------|-------------------|
| Do I do this often or just once? | One-time tasks aren't worth automating — just ask Claude to help |
| Do I enjoy this or would I delegate it? | Enjoy it = augment. Hate it = automate |
| How complex is this? | Complex tasks need to be broken into smaller steps |
| Can I explain it step-by-step? | If you can't articulate it, Claude can't do it |
| Does it need my judgment throughout? | High judgment = augment. Low judgment = automate |
| Can I define what "done" looks like? | Clear success criteria = easier to automate |
| What's the risk if Claude gets it wrong? | High risk = more oversight. Low risk = let it run |

### The 80% Rule

> "80% done by someone else is 100% awesome."

Don't aim for AI to do things perfectly. Aim for AI to get you 80% of the way there, then you polish the last 20%. This is especially true for PMM work — Claude can draft, research, and organize, but you make the final calls.

### PMM Tasks Worth Automating

Based on the pattern of what works well with AI:

**Good candidates for automation:**
- Pulling release info from Linear and summarizing it
- Drafting initial doc updates from specs
- Generating competitive research summaries
- Creating first drafts of release notes
- Formatting and organizing existing content

**Good candidates for augmentation:**
- Writing messaging and positioning (Claude drafts, you refine)
- Reviewing content for consistency with brand voice
- Brainstorming campaign ideas
- Critiquing your own work before sharing

**Keep doing yourself:**
- Final messaging decisions
- Stakeholder relationships
- Strategic prioritization
- Knowing what actually matters to your customers

---

## What's Next?

Ready to get started? Here's your path:

1. **[Getting Started Guide](getting-started.md)** — Install Claude Code and learn the basics
2. **[GrowthScript Overview](../frameworks/growthscript.md)** — Understand the framework you'll be operationalizing
3. **[/setup](../skills/setup-wizard.md)** — Connect Claude Code to your tools

Take it one step at a time. You don't need to understand everything before you start.

---

## Questions?

This toolkit was created by Taylor Berry. Reach out at taylormichellejoyce@gmail.com
