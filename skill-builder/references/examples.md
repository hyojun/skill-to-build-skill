# Example Skills for Inspiration

Here are three complete example skills — one from each category. Use these to help the user understand what a finished skill looks like.

---

## Example 1: Meeting Notes Creator (Category: "Create things")

```
---
name: meeting-notes
description: Creates clean, organized meeting notes from a conversation or rough notes. Use when someone says "write up meeting notes", "summarize this meeting", "create meeting minutes", or "turn my notes into a summary".
---

# Meeting Notes Creator

## Instructions

### Step 1: Get the raw input
Ask the user for their meeting notes or a description of what was discussed. This could be:
- Rough bullet points
- A paste of a chat transcript
- A verbal summary they type out

If they don't mention it, ask: "Who was in the meeting, and what was the main topic?"

### Step 2: Organize the notes
Sort everything into these sections:
- **Date and attendees** — who was there
- **Key topics discussed** — the main things that came up
- **Decisions made** — anything that was agreed on
- **Action items** — who needs to do what, and by when
- **Next steps** — what happens after this meeting

### Step 3: Write it up cleanly
Turn the organized notes into a clean, easy-to-read document. Use:
- Short bullet points (not long paragraphs)
- Bold text for names and deadlines
- A clear header for each section

### Step 4: Review with the user
Show the draft and ask:
- "Did I miss anything?"
- "Are the action items right?"
- "Should I change the tone (more formal or more casual)?"

Make any changes they request.

## Examples

### Example 1: Quick standup notes
**User says:** "Can you write up notes from our standup? It was me, Sarah, and Mike. I'm working on the login page, Sarah is fixing the search bug, and Mike is reviewing PRs. We need to ship by Friday."

**What to do:**
1. Create meeting notes with the three attendees
2. List each person's update as a key topic
3. Add "Ship by Friday" as a decision/deadline
4. Format cleanly

**Result:** A short, organized standup summary with clear ownership and the Friday deadline highlighted.

### Example 2: Longer planning meeting
**User says:** "Here are my rough notes from the planning meeting..." (followed by messy bullet points)

**What to do:**
1. Parse through the rough notes
2. Identify topics, decisions, and action items
3. Ask about anything unclear
4. Create a polished document

**Result:** A complete meeting summary that turns messy notes into a clear, shareable document.

## Troubleshooting

**If the notes are very short or vague:**
Ask follow-up questions: "Can you tell me more about what was decided?" or "Who's responsible for the next steps?"

**If the user wants a specific format:**
Ask them to share a sample or describe what they want, then match that format.
```

---

## Example 2: Weekly Report Generator (Category: "Automate a process")

```
---
name: weekly-report
description: Generates a weekly progress report by asking about accomplishments, blockers, and plans. Use when someone says "write my weekly report", "weekly update", "status report", "what I did this week", or "help with my weekly summary".
---

# Weekly Report Generator

## Instructions

### Step 1: Ask about this week's accomplishments
Start with: "What did you get done this week? Just list the highlights — don't worry about making it sound fancy."

Let the user list things informally. Don't rush them.

### Step 2: Ask about blockers
Ask: "Did anything slow you down or get in your way this week?"

If they say no, that's fine — skip this section in the report.

### Step 3: Ask about next week
Ask: "What are you planning to focus on next week?"

### Step 4: Ask about highlights or shout-outs (optional)
Ask: "Anything else worth mentioning? A win you're proud of, someone who helped you, or something the team should know about?"

### Step 5: Generate the report
Create a clean report with these sections:
- **Week of [date range]**
- **Accomplishments** — bullet points, past tense, specific
- **Blockers** — if any, with status (resolved/ongoing)
- **Next Week** — bullet points, clear priorities
- **Notes** — optional highlights or shout-outs

Keep the tone professional but not stiff. Match the user's voice.

### Step 6: Review and adjust
Show the draft. Ask: "How does this look? Want me to add detail anywhere or trim it down?"

## Examples

### Example 1: Engineering weekly report
**User says:** "I need to write my weekly report. I finished the payment integration, fixed three bugs, and started on the dashboard redesign. No blockers. Next week I'm focused on the dashboard."

**What to do:**
1. Expand each accomplishment into a clear bullet point
2. Note no blockers
3. List next week's focus
4. Format as a weekly report

**Result:** A polished weekly report ready to send to their manager.

### Example 2: Short and sweet
**User says:** "Weekly update: mostly meetings this week, got the proposal approved, need to start hiring."

**What to do:**
1. Turn the short summary into structured sections
2. Ask if there's anything to add about the hiring plan
3. Generate a concise report

**Result:** A brief but complete weekly update.

## Troubleshooting

**If the user gives one-word answers:**
Prompt gently: "Can you tell me a bit more about that? Even one sentence helps me write a better report."

**If the user wants a different format:**
Ask: "What does your team usually expect? I can match whatever format they use."
```

---

## Example 3: Project Board Setup (Category: "Work with a connected app")

```
---
name: project-board-setup
description: Sets up a new project board in your project management tool with tasks, labels, and team assignments. Use when someone says "set up a new project", "create a project board", "start a new project", "initialize project tasks", or "set up sprint".
---

# Project Board Setup

## Instructions

### Step 1: Understand the project
Ask the user:
- "What's the project called?"
- "Can you describe it in a sentence or two?"
- "Who's on the team?"

### Step 2: Break it into tasks
Help the user list out the main tasks or milestones. Ask:
- "What are the big things that need to get done?"
- "Can we break any of those into smaller steps?"

Aim for 5-15 tasks to start. You can always add more later.

### Step 3: Organize the tasks
For each task, figure out:
- **Who** should work on it (assign a team member)
- **Priority** — is it urgent, important, or nice-to-have?
- **Order** — what needs to happen first?

### Step 4: Create the board
Using the connected project management app:
1. Create a new project with the given name and description
2. Add each task with the right assignee and priority
3. Set up any labels or categories the team uses
4. Arrange tasks in the right order

### Step 5: Share and confirm
Show the user a summary of what was created:
- Project name
- Number of tasks
- Team assignments
- Any labels or milestones set up

Ask: "Does this look right? Want to add, remove, or change anything?"

## Examples

### Example 1: New feature project
**User says:** "Set up a project for our new mobile app feature. The team is Alex, Jordan, and Sam. We need design, development, testing, and launch tasks."

**What to do:**
1. Create a project called "Mobile App Feature" (or ask for a specific name)
2. Break into phases: Design, Development, Testing, Launch
3. Create tasks for each phase
4. Assign to team members based on their roles
5. Set priorities (design first, then development, etc.)

**Result:** A fully set up project board with 10-12 tasks, assigned to the right people, in the right order.

### Example 2: Simple task list
**User says:** "I just need a quick project board for our office move. Tasks: find movers, set a date, notify the team, pack up, move day."

**What to do:**
1. Create a project called "Office Move"
2. Add the five tasks in order
3. Ask who should be assigned
4. Set them up in the connected app

**Result:** A simple, clean project board with five tasks ready to track.

## Troubleshooting

**If the connected app isn't available:**
Let the user know: "I can't reach your project tool right now. Want me to create the task list as a document instead? You can copy it over later."

**If the user isn't sure about task breakdown:**
Help them brainstorm: "For a project like this, teams usually need tasks for [common phases]. Want to start with those?"
```
