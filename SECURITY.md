# Security & AI Usage Guidelines

Before using PMM Partner (or any AI tool with access to your systems), understand these principles.

---

## API Keys & Credentials

- **Never paste API keys, passwords, or secrets into AI prompts**
- If you accidentally expose a key, **revoke it immediately** and generate a new one
- Store credentials in environment variables, not in files or chat
- When setting up MCP connections, the keys are stored locally - keep your machine secure

---

## Working with Sensitive Data

One of the biggest advantages of Claude Code is that it can work with your real data - customer info, CRM records, internal docs - through **approved integrations** like HubSpot, Salesforce, or Notion MCP connections.

### This is OK:
- Accessing customer data through **sanctioned MCP integrations** (these use your existing permissions and audit trails)
- Querying your CRM through an approved connection
- Working with data inside systems your IT/Security team has vetted

### This is NOT OK:
- Copy-pasting raw customer data into unvetted AI tools
- Uploading CSVs of sensitive data to random websites
- Bypassing your company's access controls
- Sharing credentials so others can access data they shouldn't

### The Key Difference:
**Approved integrations** = data stays within controlled systems with audit trails
**Copy-paste into chat** = data leaves your controlled environment

### Still Avoid in Any AI Prompt:
- Production database credentials or API secrets
- Passwords or authentication tokens
- Anything that would let someone impersonate you or access systems

**Follow your company's data handling policies.** If your organization has approved certain integrations, use those. If you're unsure what's approved, ask IT or Security.

---

## MCP Connections = Real Access (That's the Point)

When you connect Claude Code to tools like Notion, Linear, HubSpot, or Salesforce:

- It has **real access** to your data - that's what makes it powerful
- It uses **your existing permissions** - you can only access what you could access anyway
- Actions are auditable in the connected systems
- It can create, edit, and delete things on your behalf

### Best Practices:
- **Understand what you're connecting** - know what data the integration can access
- **Review before confirming** - especially for edits or deletions
- **Use integrations IT/Security has approved** - these have been vetted
- **Start with read-heavy workflows** if you're learning

**The value is working through your systems, not around them.**

---

## AI Can Be Confidently Wrong

AI tools are powerful but imperfect:

- Always verify before running destructive commands
- Don't blindly execute code or commands you don't understand
- If Claude says "Let me delete that for you" → **pause and think**
- Ask "what will this command do?" before approving anything you're unsure about
- Review changes before committing or publishing

---

## Data & Privacy

### Anthropic's Policies
- Claude Code conversations are **not used for model training** by default
- Check your plan's data retention settings at [anthropic.com](https://anthropic.com)
- Enterprise plans have additional privacy controls

### Your Company's Policies
- Check if your organization has an AI usage policy
- Know who to ask if you're unsure (usually IT, Security, or Compliance teams)
- When in doubt, default to caution

---

## Best Practices

1. **Start small** - Connect one tool at a time, understand what access you're granting
2. **Review before confirming** - Read what Claude is about to do before saying yes
3. **Use test/staging environments** - Don't experiment in production
4. **Keep credentials secure** - Treat API keys like passwords
5. **Ask questions** - If something feels risky, ask before proceeding

---

## If Something Goes Wrong

- **Exposed a credential?** Revoke it immediately and generate a new one
- **Deleted something important?** Check for backups, version history, or trash folders
- **Unsure about an action Claude took?** Review the change history in your tool
- **Security concern?** Report it to your IT/Security team

---

## Questions?

If you're unsure whether something is safe to share with AI tools, ask your Security or IT team first. It's always better to check than to clean up a breach.
