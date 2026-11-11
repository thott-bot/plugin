<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset=".github/media/mark-dark.svg">
  <img src=".github/media/mark-light.svg" width="88" alt="thott.bot">
</picture>

# thott.bot

**World of Warcraft: Forever for ChatGPT, Claude and any AI: items, quests, talents, maps and guides.**<br>
Everything about WoW Forever, in the chat app you already use.

<a href="https://thott.bot/ai"><img src=".github/media/ai-questions.avif" width="100%" alt="An AI chat with thott.bot answering five World of Warcraft: Forever questions: where to get a sleeping bag, the most popular Retribution Paladin builds, what to cook, new gear for a level 28 warrior, and what's new for warriors at 20."></a>

**[Add to ChatGPT](https://chatgpt.com/plugins/plugin_asdk_app_6ac3efb508348191a717c69b6e2f775d)** · **[Different AI?](#which-ai-apps-does-it-work-with)** · **[thott.bot](https://thott.bot)**<br>
**About 20 free questions** a month, no card needed.

</div>

## Close your tabs.

Anything you'd look up is already in your chat.

- **Never lagging.** thott.bot tracks every change to the game within minutes of it landing, and Blizzard's own news
  and posts.
- **Straight from the game.** Every number and tooltip comes from Blizzard's game files for the build you're playing.
- **Drawn in the chat.** In ChatGPT and Claude, talent trees, tooltips, quest chains and maps appear right in the
  conversation.

## What it knows

- **Every update:** each new build of the game and everything it changed, tracked automatically within minutes of it
  landing, plus Blizzard's news and developer posts from the official forums.
- **Classes:** every class, race and racial, ability and talent, and what Forever changed from Classic.
- **Builds:** the talent builds players are running right now, and each spec's talent pick rates.
- **Gear:** every item, item set and recipe, with where it drops and who sells it.
- **Quests:** every quest, its chain, route and rewards, and the NPCs and objects along the way.
- **The world:** zones and maps, flight paths, dungeons and raids with their bosses, and battlegrounds.
- **Guides:** leveling and profession guides.
- **Professions:** every profession, riding and other skills.
- **Collections:** mounts, companion pets, toys, achievements, titles, reputations, currencies, holidays and the
  Legacy system.
- **Combat:** buffs and debuffs, pet abilities and diminishing returns.
- **The interface:** every setting, key binding, chat command and character customization option.
- **Addons:** the addon API, and which addons are banned.

## Ask the way you already do

- Where do I get the sleeping bag in WoW Forever?
- What's the most popular Fire Mage build in WoW Forever right now?
- How do I level cooking cheaply in WoW Forever?
- What new gear should my level 28 warrior look out for in WoW Forever?
- I play a Paladin. What changed for me in WoW Forever this week?
- Build me a cooldown-tracker addon. What can the Forever client's API do in combat?

## Can't my AI already do this?

Yeah, badly. Your AI learned WoW once, the day its training stopped, and it has been behind on every change since. To
cover the gap, it searches the web and stitches together SEO spam, forum guesses and guides for older patches.
thott.bot connects it straight to the game, current within minutes of every change.

## Which AI apps does it work with?

Any app that supports MCP, including ChatGPT and Codex with the official thott.bot plugin, Claude on every plan,
Claude Code, Cursor and Hermes.

The first connection opens a sign-in page (Discord, Google or email), which creates a free account.

### ChatGPT and Codex

Install the [official thott.bot plugin](https://chatgpt.com/plugins/plugin_asdk_app_6ac3efb508348191a717c69b6e2f775d),
then sign in.

### Claude

[Add thott.bot to Claude](https://claude.ai/customize/connectors?modal=add-custom-connector&connectorName=thott.bot&connectorUrl=https%3A%2F%2Fmcp.thott.bot%2Fmcp)
opens Claude's Add custom connector dialog with the name and address filled in. Select Add, then Connect, and sign in.

### Claude Code

```
claude mcp add --transport http --scope user thott https://mcp.thott.bot/mcp
claude mcp login thott
```

### Codex CLI

```
codex mcp add thott --url https://mcp.thott.bot/mcp
```

That opens the sign-in itself; if it doesn't, run `codex mcp login thott`.

### Cursor

[Add thott.bot to Cursor](https://cursor.com/install-mcp?name=thott&config=eyJ1cmwiOiJodHRwczovL21jcC50aG90dC5ib3QvbWNwIn0%3D)
opens Cursor with thott.bot filled in. Then sign in.

### Hermes

```
hermes mcp add thott --url https://mcp.thott.bot/mcp --auth oauth
```

That opens the sign-in itself; if it doesn't, run `hermes mcp login thott`.

### Any other app

Add `https://mcp.thott.bot/mcp` wherever it adds a remote MCP server (Streamable HTTP, OAuth sign-in).

[Steps for each app](https://thott.bot/setup)

## Is this an MCP server?

Yes, a remote MCP server at `https://mcp.thott.bot/mcp`. Your AI signs in with OAuth and gets read-only tools to
search the game, open full entries, track every change between builds, and draw answers as interactive displays.

## Is this just scraped from other sites?

No. thott.bot reads Blizzard's own game files, news and forum posts. Community data, like quest and loot details, comes
only from projects that explicitly allow it to be used this way, and it's always credited.

## Does thott.bot read my chats or train AI on them?

thott.bot only sees what your AI sends when it looks something up: the short search it writes and basic details like
which app and model. It never sees your conversation, your messages or your AI's replies, and none of it is used to
train AI models.

## What does it cost?

It's free for about 20 questions each month, no card needed. [Unlimited](https://thott.bot/plans) has no monthly limit.

## In your game, too.

Bring your AI into Azeroth with [thott.bot chat](https://github.com/thott-bot/chat), the free addon.

## What's in this repository

- `.cursor-plugin/` and `mcp.json`: the Cursor plugin.
- `hermes/`: the Hermes plugin.

There's no server code here: the plugins point your app at `https://mcp.thott.bot/mcp`.
