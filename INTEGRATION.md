# Claude Content Writer Agent Integration Guide

## Overview

This project is configured to use the **Claude Content Writer** agent from `sociilabs/claude-content-writer`. This agent provides a comprehensive system for generating high-quality, human-sounding blog content.

## Installation

The Claude Content Writer skill needs to be installed via Claude Code:

```bash
npx skills add sociilabs/claude-content-writer
```

## Key Features

### 1. Profile-Based Voice Calibration
The agent learns your writing style through profiles stored in the `profiles/` directory. Each profile defines:
- Tone and audience
- Formality and vocabulary level
- Sentence and paragraph structure
- Personalization preferences

Default profile: `profiles/default-profile.json`

### 2. Five-Phase Workflow

The agent follows a structured approach:

1. **Discuss** - Understand requirements and context
2. **Plan** - Outline content structure and key points
3. **Execute** - Write the initial draft
4. **Verify** - Review quality, SEO, and humanization
5. **Ship** - Finalize and prepare for publishing

### 3. Content Types Supported

- Blog Articles
- LinkedIn Posts
- Email Newsletters
- Landing Pages
- Case Studies

### 4. Quality Assurance Features

- **SEO Optimization** - Automatic keyword optimization
- **AI Pattern Detection** - Removes artificial-sounding language
- **Humanization** - Adds personal examples and natural flow
- **Tone Consistency** - Maintains voice across all content

## Usage Examples

### Generate a Blog Article

```
Use the Claude Content Writer agent to write a blog article about:
- Topic: "Best Practices for Remote Team Management"
- Target Audience: HR professionals and team leads
- Length: 1500 words
- Profile: default-profile
- Include: Table of contents, examples, call-to-action
```

### Generate a LinkedIn Post

```
Use the Claude Content Writer agent to write a LinkedIn post:
- Topic: "5 Tips for Effective Leadership"
- Tone: Inspiring and professional
- Length: 150-200 words
- Profile: default-profile
- Include: Hook, key points, call-to-engagement
```

### Generate a Newsletter

```
Use the Claude Content Writer agent to write an email newsletter:
- Topic: "Monthly Product Updates"
- Audience: Product users
- Length: 300-400 words
- Profile: default-profile
- Format: Introduction, 3 key updates, closing
```

## Configuration

### Project Settings

Edit `.claude-code-config.json` to customize:
- Output directories
- Default profiles
- SEO optimization settings
- AI pattern detection sensitivity
- Tone enforcement rules

### Writing Profiles

Create new profiles by copying `profiles/default-profile.json` and customizing:

```json
{
  "name": "Technical Profile",
  "style": {
    "formality": "formal",
    "vocabulary": "technical",
    "useConversationalLanguage": false
  },
  // ... other settings
}
```

## Directory Structure

```
blog_writer/
├── content/
│   ├── blog/              # Generated blog articles
│   ├── social/            # Social media content
│   └── newsletters/       # Email newsletter content
├── profiles/
│   └── default-profile.json
├── .claude-code-config.json
├── CLAUDE.md
├── INTEGRATION.md         # This file
├── package.json
└── README.md
```

## Next Steps

1. Install the skill: `npx skills add sociilabs/claude-content-writer`
2. Review the profiles in `profiles/` directory
3. Create custom profiles for different content types
4. Start generating content using the agent

## Support

For more information about the Claude Content Writer agent, visit:
https://github.com/sociilabs/claude-content-writer

For Claude Code documentation:
https://github.com/anthropics/claude-code
