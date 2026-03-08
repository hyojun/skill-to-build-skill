# Skill Builder

A skill that helps you create new skills for Claude — step by step, no technical knowledge required.

Instead of reading documentation and figuring out file formats, just tell Claude what you want it to do. The Skill Builder walks you through the entire process in a friendly, conversational way and generates a ready-to-use skill at the end.

## What It Does

The Skill Builder guides you through 6 simple phases:

1. **What do you want Claude to do?** — Describe your idea in plain language
2. **Name and describe it** — Create a name and short pitch for your skill
3. **Outline the steps** — Map out what Claude should do, in order
4. **Add examples** — Write example conversations so Claude knows what to expect
5. **Review it** — Walk through a checklist to catch any issues
6. **Get your skill** — Receive the finished skill file with installation instructions

## Installation

### Claude.ai

1. Download or clone this repository
2. Zip the `skill-builder` folder
3. Go to **Settings > Capabilities > Skills** in Claude.ai
4. Click **Upload skill** and select the zip file

### Claude Code

Place the `skill-builder` folder in your Claude Code skills directory:

```bash
# Clone the repo
git clone https://github.com/Swingvy/skill-to-build-skill.git

# Copy the skill folder to your project
cp -r skill-to-build-skill/skill-builder /path/to/your/project/.claude/skills/
```

Or install it globally:

```bash
cp -r skill-to-build-skill/skill-builder ~/.claude/skills/
```

## Usage

Once installed, just ask Claude to help you build a skill. Any of these will work:

- "Help me build a skill"
- "I want to create a skill"
- "Help me teach Claude to do X"
- "I want Claude to automate my weekly reports"
- "Make a skill for generating meeting notes"

Claude will take it from there — asking questions, guiding you through each phase, and generating the finished skill file when you're done.

## What's Inside

```
skill-builder/
├── SKILL.md                    # Main skill — the interactive wizard
└── references/
    ├── examples.md             # 3 example skills for inspiration
    ├── checklist.md            # Review checklist used in Phase 5
    └── troubleshooting.md      # Common problems and fixes
```

## Built Based On

This skill is built based on [The Complete Guide to Building Skills for Claude](https://claude.com/blog/complete-guide-to-building-skills-for-claude) — Anthropic's official guide covering everything from skill structure and design patterns to testing and distribution. The Skill Builder packages that knowledge into an interactive, beginner-friendly wizard so you don't have to read the guide yourself.

## Who Is This For

Anyone who wants to create a skill for Claude but doesn't want to deal with technical details. The Skill Builder handles all the formatting and structure — you just describe what you want in plain language.

## License

MIT
