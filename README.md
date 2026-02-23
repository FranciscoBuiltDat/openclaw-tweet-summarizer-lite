# Tweet Summarizer Lite

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

An **OpenClaw agent skill** — fetch and summarize single tweets from Twitter/X using natural language. Just paste a tweet URL or ask your agent to grab it.

## What It Does

- 🐦 **Fetch any tweet** — paste a URL and your agent reads it instantly
- 📊 **Auto-summary** — key points extracted automatically
- 🔍 **Search saved tweets** — find tweets by text, author, or date
- 💾 **Persistent storage** — tweets saved locally for later lookup

## How to Use

Once installed, just talk to your agent naturally:

> *"What does this tweet say?"* → paste an x.com URL  
> *"Grab this tweet and save it"*  
> *"Search my saved tweets for anything about AI agents"*  
> *"Find tweets I saved from @karpathy"*  
> *"What have I saved since February?"*

Your agent handles everything — no commands needed.

## Installation

Install via [ClawHub](https://clawhub.ai) or clone manually:

```bash
git clone https://github.com/FranciscoBuiltDat/openclaw-tweet-summarizer-lite.git
```

## Prerequisites

Requires the [`bird`](https://github.com/steipete/bird) CLI and valid Twitter session cookies.

```bash
npm install -g @steipete/bird
```

Set your credentials (see [SECURITY.md](SECURITY.md) for how to get these):

```bash
export AUTH_TOKEN="your_auth_token"
export CT0="your_ct0_token"
```

## Storage

Tweets are saved to `~/.openclaw/workspace/data/tweets/` as JSON, with a master `index.json` for fast search.

## Pro Version

Need threads, user timelines, collections, or tags? Upgrade to [tweet-summarizer-pro](https://github.com/FranciscoBuiltDat/openclaw-tweet-summarizer-pro):

- 🧵 Full thread fetching + thread summaries
- 📂 Custom collections with archive/restore
- 👤 User and home timeline fetching
- 🏷️ Tags and advanced search filters

## Contributing

Contributions welcome! Please read [SECURITY.md](SECURITY.md) before contributing.

## License

MIT — see [LICENSE](LICENSE)
