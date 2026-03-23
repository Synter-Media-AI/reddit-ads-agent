# Reddit Ads MCP Starter Kit — Manage Reddit Ads with AI

[![MCP Compatible](https://img.shields.io/badge/MCP-compatible-blue)](https://modelcontextprotocol.io)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform: Reddit Ads](https://img.shields.io/badge/Platform-Reddit%20Ads-FF4500)](https://ads.reddit.com)

**Reach niche communities where people actually trust recommendations.** Open this repo in Amp, Cursor, or VS Code and manage Reddit ad campaigns with AI — target by subreddit, interest, and community behavior with ads that feel native to the platform.

---

## Why Reddit Ads + AI?

Reddit is the internet's town square — 1.7 billion monthly visits across 100,000+ active communities. Unlike any other platform, Reddit users self-organize by interest into subreddits: r/startups, r/personalfinance, r/gaming, r/homeimproving, r/skincare. This creates advertising niches that don't exist anywhere else.

The challenge? Reddit users are notoriously ad-allergic. Overtly promotional content gets downvoted into oblivion. The ads that work on Reddit look and feel like regular posts — genuine, helpful, slightly irreverent. This requires a fundamentally different creative approach than Google or Meta.

An AI agent helps you navigate Reddit's unique culture. It knows which subreddits to target, writes copy that feels native, and manages campaigns through Reddit's v3 API — which is complex and poorly documented.

**Best for:** Tech products, gaming, niche hobbies, finance apps, developer tools, ecommerce in passionate niches (coffee, keyboards, skincare, fitness).

---

## Quick Start (30 Seconds)

### Amp / Cursor / VS Code (Copilot)

1. **Get a free API key** at [syntermedia.ai/developer](https://syntermedia.ai/developer)
2. **Set the key:**
   ```bash
   export SYNTER_API_KEY=syn_your_key_here
   ```
3. **Open this repo** in your editor
4. **Start chatting** — MCP tools are pre-configured in `.mcp.json`

### Claude Desktop

Copy `claude_desktop_config.json` to your Claude config directory and replace the API key:

- **macOS:** `~/Library/Application Support/Claude/claude_desktop_config.json`
- **Windows:** `%APPDATA%\Claude\claude_desktop_config.json`

---

## What You Can Do

| Capability | Example |
|-----------|---------|
| **Create Promoted Posts** | "Create a promoted post about our mechanical keyboard in r/MechanicalKeyboards style" |
| **Subreddit Targeting** | "Target r/startups, r/SaaS, and r/smallbusiness for our project management tool" |
| **Interest Targeting** | "Target people interested in personal finance and investing" |
| **Conversation Ads** | "Set up a conversation-style ad that invites discussion" |
| **Community Research** | "Which subreddits would be most relevant for a fitness app?" |
| **Campaign Activation** | "Launch a CONVERSIONS campaign with $50/day budget targeting tech subreddits" |
| **Performance Reports** | "Which subreddits are driving the most conversions?" |
| **CTA Optimization** | "Which call-to-action ('Learn More' vs 'Sign Up') performs better?" |
| **Geo Targeting** | "Only show ads to users in the US and Canada" |
| **Budget Management** | "Increase budget on our top-performing ad group by 30%" |

---

## Example Conversations

### 1. Creating a Native-Feeling Promoted Post

> **You:** I'm launching a new budgeting app. I want to advertise on Reddit but I know Redditors hate ads.
>
> **Agent:** You're right to be cautious. Reddit ads that look like ads get destroyed. The ones that work provide genuine value.
>
> Here's my approach for your budgeting app:
>
> **Don't do this:** "🚀 BudgetPro — The #1 Budgeting App! Download Now! 💰"
>
> **Do this instead:** "I built a budgeting app because YNAB didn't work for my ADHD brain — here's what's different"
>
> This works because:
> - It's personal and authentic (Reddit values real stories)
> - It acknowledges an existing popular tool (YNAB) without bashing it
> - It promises useful differentiation
> - The tone matches how Redditors naturally post
>
> **Targeting:**
> - r/personalfinance, r/budgeting, r/ynab, r/frugal, r/povertyfinance, r/ADHD
> - Interest: Personal Finance, Budgeting
> - Geo: US, Canada, UK, Australia
> - Budget: $30/day
>
> **You:** I love the angle. But we're not specifically for ADHD — should I mention it?
>
> **Agent:** Good point. Let me rework: "I tried every budgeting app and they all assumed I'd track every coffee. So I built one that works with just your bank connection — no manual entry."
>
> This hits the same authentic tone without the ADHD angle. Target r/personalfinance and r/budgeting where "too much manual work" is a universal complaint.

### 2. Subreddit Performance Deep Dive

> **You:** I'm targeting 12 subreddits. Which ones are actually working?
>
> **Agent:** Pulling subreddit-level performance for the last 14 days...
>
> | Subreddit | Spend | CTR | CPA | Conversions |
> |---|---|---|---|---|
> | r/startups | $180 | 1.8% | $22.50 | 8 |
> | r/SaaS | $140 | 2.3% | $17.50 | 8 |
> | r/smallbusiness | $210 | 0.9% | $42.00 | 5 |
> | r/Entrepreneur | $320 | 0.7% | $64.00 | 5 |
> | r/webdev | $95 | 3.1% | $11.88 | 8 |
> | r/programming | $280 | 0.4% | $140.00 | 2 |
>
> **Clear winners:** r/webdev ($11.88 CPA, 3.1% CTR) and r/SaaS ($17.50 CPA). These communities are engaged and high-intent.
>
> **Cut immediately:** r/programming ($140 CPA) and r/Entrepreneur ($64 CPA). r/programming is too broad — developers browsing code discussions aren't in a buying mindset. r/Entrepreneur attracts side-hustlers, not SaaS buyers.
>
> **Recommendation:** Reallocate r/programming and r/Entrepreneur budget to r/webdev and r/SaaS. Expected result: ~30% lower blended CPA.

### 3. Conversation-Style Ad Strategy

> **You:** What's a "conversation ad" on Reddit?
>
> **Agent:** It's Reddit's most native ad format. Instead of a display ad, you create a promoted post that invites genuine discussion. The comments section becomes part of the ad experience.
>
> **How to do it well:**
>
> Post: "We analyzed 10,000 A/B tests across SaaS landing pages. Here are the 3 changes that actually moved the needle (data inside)"
>
> Then in the comments, your brand account shares:
> - Finding 1: Social proof above the fold → +34% conversion
> - Finding 2: Benefit headlines outperform feature headlines 4:1
> - Finding 3: Removing navigation links → +12% conversion
>
> Real users start commenting with their own experiences. The thread becomes genuinely useful. Your brand is positioned as a helpful expert, not a pushy advertiser.
>
> **Key rules:**
> - Actually engage in the comments (don't post and ghost)
> - Accept constructive criticism gracefully
> - Never delete negative comments (Redditors notice and it backfires)
> - Share genuinely useful data — don't hold everything behind a paywall

### 4. Reddit Pixel & Conversion Tracking

> **You:** I want to track signups from Reddit Ads. How do I set up conversion tracking?
>
> **Agent:** Reddit has its own conversion pixel. Here's the setup:
>
> 1. **Install the Reddit Pixel** on your website (goes in the `<head>` tag)
> 2. **Create conversion events:** SignUp, Purchase, Lead, etc.
> 3. **Set up the Conversions API (CAPI)** for server-side tracking (recommended — catches conversions the browser pixel misses)
>
> For your campaign, I'll:
> - Create a "SignUp" conversion event
> - Set the ad group to optimize for SIGN_UP conversions
> - Use MAXIMIZE_VOLUME bid strategy with $30/day budget
>
> **Important Reddit tracking quirk:** The Reddit Pixel uses `rdt_cid` for click attribution and `_rdt_uuid` for view-through. Make sure both cookies are captured. The Synter MCP handles CAPI automatically.

### 5. AMA-Style Promotion

> **You:** Our CEO wants to do an AMA on Reddit. Can we promote it?
>
> **Agent:** Great idea — AMAs are Reddit's most authentic format. Here's how to maximize it:
>
> **Pre-AMA (1 week before):**
> - Create a promoted post announcing the AMA: "I'm [Name], CEO of [Company]. I've spent 10 years building developer tools. AMA next Thursday at 2pm ET in r/startups"
> - Target: r/startups, r/SaaS, r/programming, r/cscareerquestions
> - Budget: $200 total (5-day run)
>
> **During AMA:**
> - Promote the live AMA thread to the same subreddits
> - Budget: $100 for the day (concentrate impressions)
>
> **Post-AMA:**
> - Promote a "Highlights from our AMA" follow-up post
> - Include best Q&A pairs and link to the full thread
> - This has longer shelf life than the live event
>
> **Tips for the AMA itself:**
> - Answer honestly — Redditors have BS detectors
> - Give real numbers when possible ("we grew from $0 to $2M ARR in 18 months")
> - Don't dodge tough questions
> - Stay for at least 2 hours
> - Your CEO should use their personal Reddit account, not a brand account

---

## Reddit Ads Tips from the Pros

1. **Be authentic or be destroyed.** Redditors can spot a corporate shill from a mile away. Your ads should sound like a person, not a brand. First person, casual tone, real stories.
2. **Target by subreddit, not interest.** Subreddit targeting is Reddit's superpower. r/MechanicalKeyboards is 10x more specific than "Keyboard Interest." Start with 5-8 specific subreddits.
3. **Promoted posts should feel native.** Your ad should be indistinguishable from a regular post in the subreddit. Study what gets upvoted in your target subreddits and mirror that format.
4. **Comments matter more than impressions.** A promoted post with 50 genuine comments outperforms one with 50,000 impressions and 0 comments. Engage with every commenter.
5. **Use "Learn More" not "LEARN_MORE."** Reddit's CTA values use natural capitalization. Getting this wrong causes API errors.
6. **Budget minimum: $5/day.** Reddit's minimum is low, but $20-30/day per ad group is more realistic for gathering enough data. Start there and scale winners.
7. **Never use hashtags or emojis in headlines.** This screams "ad" on Reddit. Clean, plain text performs best.

---

## FAQ

### Is there an MCP for Reddit Ads?
Yes — this repo. It pre-configures the Synter MCP server for Reddit Ads campaign management. Works with Amp, Cursor, VS Code, and Claude Desktop.

### Can AI write Reddit-native ad copy?
Yes. The agent understands Reddit's culture and can write promoted posts that feel like organic content — first person, authentic tone, value-driven headlines.

### What subreddits can I advertise in?
Most subreddits with 10,000+ subscribers accept promoted posts. You can target specific subreddits, interest categories, or communities. The agent can recommend subreddits based on your product.

### Do Reddit Ads actually work?
For the right products, absolutely. Tech products, gaming, personal finance, niche ecommerce — these categories see strong performance. The key is native creative that adds value to the community.

### What's the Reddit Conversions API?
Server-side conversion tracking that sends events directly from your server to Reddit. It's more reliable than the browser pixel and catches conversions lost to ad blockers and cookie restrictions.

### Can I promote my own Reddit posts?
Not directly. Promoted posts are created through the Reddit Ads API and appear as "Promoted" in feeds. They can link to your website, app, or a Reddit thread.

---

## Related Repos

- [google-ads-agent](https://github.com/Synter-Media-AI/google-ads-agent) — Search intent capture
- [meta-ads-agent](https://github.com/Synter-Media-AI/meta-ads-agent) — Facebook & Instagram reach
- [x-ads-agent](https://github.com/Synter-Media-AI/x-ads-agent) — Twitter/X promotion
- [conversion-tracking-agent](https://github.com/Synter-Media-AI/conversion-tracking-agent) — Reddit Pixel setup
- [cross-platform-ads-agent](https://github.com/Synter-Media-AI/cross-platform-ads-agent) — Multi-channel management
- [audience-sync-agent](https://github.com/Synter-Media-AI/audience-sync-agent) — Sync audiences to Reddit

---

## License

MIT — see [LICENSE](LICENSE) for details.

Built by [Synter](https://syntermedia.ai) · [Get API Key](https://syntermedia.ai/developer) · [Documentation](https://syntermedia.ai/docs)
