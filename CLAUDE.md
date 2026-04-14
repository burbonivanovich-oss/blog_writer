# Blog Writer Project

## Overview
This project integrates the Claude Content Writer agent for high-quality blog content generation.

## Setup

The Claude Content Writer skill is integrated via Claude Code. The skill provides:

- **Profile-based voice calibration** - Captures unique writing style
- **Five-phase workflow** - Discuss, Plan, Execute, Verify, Ship
- **SEO optimization** - Built-in content optimization
- **AI pattern detection** - Removes artificial-sounding language
- **Multiple content types** - Blog articles, LinkedIn posts, newsletters, landing pages, case studies

## Installation

To use the Claude Content Writer agent in this project:

```bash
# Install the skill
npx skills add sociilabs/claude-content-writer
```

## Usage

Once installed, you can use the content writer agent through Claude Code's skill system or directly invoke it for content generation tasks.

## Project Structure

- `package.json` - Project dependencies
- `CLAUDE.md` - Project configuration (this file)
- `.claude-code/` - Claude Code configuration directory
