# Common Problems and How to Fix Them

If something isn't working with the skill, check these common issues first.

---

## "Claude doesn't use my skill when I ask it to"

**What's happening:** Claude doesn't recognize that your skill is the right one for the job.

**How to fix it:**
- Check the description — does it include the kind of things people would actually say? For example, if your skill creates meeting notes, the description should mention phrases like "write up meeting notes", "summarize this meeting", and "meeting minutes".
- Make the description more specific. "Helps with documents" is too vague. "Creates formatted meeting notes from rough bullet points" is much better.
- Try asking Claude: "When would you use the [skill name] skill?" — Claude will tell you what it thinks the skill is for, and you can adjust if it's off.

## "Claude uses my skill when it shouldn't"

**What's happening:** The description is too broad, so Claude thinks your skill applies to things it wasn't meant for.

**How to fix it:**
- Make the description more specific about what the skill is for AND what it's not for.
- For example: "Creates weekly progress reports for engineering teams. Use for weekly updates and status reports. Not for meeting notes or project documentation — use those skills instead."

## "Claude doesn't follow the steps correctly"

**What's happening:** The instructions might be unclear or too complex.

**How to fix it:**
- Break big steps into smaller ones. Instead of "Process the data and create the report", split it into "Step 1: Read the data" and "Step 2: Create the report."
- Put the most important instructions at the top — Claude pays the most attention to things near the beginning.
- Use numbered lists instead of paragraphs. Claude follows numbered steps more reliably.
- Add specific details. Instead of "format it nicely", say "use bullet points, bold headers, and keep each item to one line."

## "I can't upload my skill"

**What's happening:** Usually a file naming issue.

**How to fix it:**
- Make sure the main file is called exactly `SKILL.md` — capital S, K, I, L, L, then a dot, then lowercase md. No other spelling works.
- Make sure the folder name is all lowercase with dashes (like `my-skill-name`). No spaces, no capital letters.
- The settings at the top of the file need to start and end with three dashes on their own line, like this:

```
---
name: my-skill-name
description: What it does and when to use it.
---
```

- Make sure there are no angle brackets (`<` or `>`) anywhere in the settings at the top. These aren't allowed for security reasons.

## "The skill works but the results aren't great"

**What's happening:** The skill needs refinement.

**How to fix it:**
- Add more examples. The more examples you give Claude, the better it understands what you want.
- Be more specific in your steps. Instead of "write a good summary", say "write a 3-5 sentence summary that highlights decisions and action items."
- Add a quality check step at the end: "Before sharing the result, review it to make sure [specific criteria]."
- Test with different requests and see where it falls short, then add instructions for those cases.

## "My skill is too long and Claude seems to lose track"

**What's happening:** Too much information in one file.

**How to fix it:**
- Keep the main skill file focused on the core steps (aim for under 200 lines).
- Move detailed reference material into separate files in a `references/` folder.
- Claude will look at those extra files when it needs them, but won't get overwhelmed by reading everything at once.

## "I want to update my skill"

**How to do it:**
1. Edit the `SKILL.md` file with your changes
2. Re-upload the skill folder (you may need to remove the old version first)
3. Test with a few requests to make sure the changes work as expected

Skills are meant to be improved over time. Don't worry about getting it perfect on the first try — update it as you learn what works and what doesn't.
