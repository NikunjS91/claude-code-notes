# Plugins in Claude Code + Claude Code Notes

## What Are Plugins?

Packing and distributing a setup (skills, commands, tools) is called a **plugin**. Claude Code has a **marketplace** system for discovering and installing plugins.

A marketplace is a GitHub repo containing a `marketplace.json` file that lists available plugins.

---

## Types of Marketplaces

| Type | Description | Examples |
|------|-------------|---------|
| **Official** (`claude-plugins-official`) | Pre-added with Claude Code, curated by Anthropic | Vercel, Railway, GitHub, Supabase |
| **Third-party** | Any GitHub repo with a `marketplace.json` | Team-internal, company org, community |

Anyone can create a third-party marketplace — a team lead could publish one for their team, or a company for internal tooling.

---

## Using /plugins in Claude Code

| Step | Action |
|------|--------|
| 1 | Run `/plugins` in Claude Code |
| 2 | Go to **Discover** section to find official marketplaces |
| 3 | Click **Add Marketplace**, paste the URL, hit Enter |
| 4 | Browse and install plugins from the marketplace |

---

## Deploying to Railway (Example)

### Setup

```bash
# Install Railway CLI
npm install -g @railway/cli

# Authenticate
railway login
railway whoami
```

### Install Railway Plugin

```
/plugin marketplace add railwayapp/railway-skills
/plugin install railway@railway-skills
```

### Deploy

Once the plugin is installed, prompt Claude Code:

> Deploy this Flask app to Railway and give me a public URL

---

*Source: [Plugins in Claude Code + Claude Code Notes.txt](Plugins%20in%20Claude%20Code%20+%20Claude%20Code%20Notes.txt)*
