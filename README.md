# Blog Writer

A content creation project leveraging the Claude Content Writer agent for high-quality, human-sounding blog content generation.

## Features

- **AI-powered Content Generation** - Uses Claude's advanced language models
- **Writing Style Calibration** - Adapts to your unique voice and tone
- **Multi-format Support** - Blog articles, LinkedIn posts, newsletters, landing pages, case studies
- **Quality Assurance** - Built-in SEO optimization and AI pattern detection
- **Structured Workflow** - Discuss → Plan → Execute → Verify → Ship

## Quick Start

1. Clone this repository
2. Install dependencies:
   ```bash
   npm install
   ```

3. Add the Claude Content Writer skill:
   ```bash
   npx skills add sociilabs/claude-content-writer
   ```

4. Start creating content using the agent

## Project Structure

```
blog_writer/
├── CLAUDE.md           # Claude Code configuration
├── package.json        # Project dependencies
├── README.md          # This file
├── content/           # Generated and managed content
│   ├── blog/          # Blog articles
│   ├── social/        # Social media posts
│   └── newsletters/   # Email newsletters
└── profiles/          # Writing style profiles
```

## Integration with Claude Code

This project is configured to work seamlessly with Claude Code. The Claude Content Writer agent provides enhanced capabilities for:

- Generating content that sounds human, not AI-generated
- Maintaining consistent voice across multiple pieces
- Optimizing content for SEO and readability
- Detecting and removing artificial language patterns

## Documentation

See `CLAUDE.md` for detailed configuration and usage instructions.
