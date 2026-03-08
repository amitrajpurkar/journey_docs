# 🚀 Claude Code Upskill Journey — Two-Week Plan

> **Learner profile:** Complete beginner · Casual coder · Goal: Build CRUD web apps & data analysis tools
> **Schedule:** Mon–Fri 30 min (6–8 pm) · Sat & Sun 60 min each
> **Total learning time:** ~11 hours over 14 days

---

## 🗺️ Learning Roadmap at a Glance

```
Week 1 — Foundations
├── Day 1  Install, first run, understand what Claude Code is
├── Day 2  CLAUDE.md — your project memory file
├── Day 3  Anthropic Academy: Claude Code in Action (Part 1)
├── Day 4  Anthropic Academy: Claude Code in Action (Part 2)
├── Day 5  Plan Mode + Peter Yang's Movie App tutorial
├── Day 6  (Saturday) Nick Saraev masterclass — core workflow sections
└── Day 7  (Sunday) Build Your First CRUD App (hands-on project)

Week 2 — Power Features
├── Day 8  Rules, Skills & SKILL.md deep dive
├── Day 9  Anthropic Academy: Claude Code Skills course
├── Day 10 SpecKit — Spec-Driven Development workflow
├── Day 11 SpecKit + Claude workflows combined (fly-by-wire)
├── Day 12 (Saturday) Sabrina Ramonov full course — Skills & hooks
└── Day 13 (Sunday) Capstone: Data Analysis Web App with full workflow
    Day 14 Review, reflect, configure your permanent environment
```

---

## 📚 Master Resource List

### Anthropic Academy (Free — requires email signup)
| Course | URL | Priority |
|--------|-----|----------|
| Claude Code in Action | https://anthropic.skilljar.com/claude-code-in-action | ⭐ Must |
| Claude Code Skills | https://anthropic.skilljar.com | ⭐ Must |
| MCP Development | https://anthropic.skilljar.com | Optional Week 3+ |
| All 13 courses index | https://anthropic.skilljar.com/ | Bookmark |

> Also available on Coursera: **Claude Code in Action** — search at coursera.org

### YouTube / Video Tutorials
| Resource | Length | Best For |
|----------|--------|----------|
| **Peter Yang** — Build a Movie App in 15 Min | 17 min | First hands-on build |
| **Sabrina Ramonov** — Full Course (Claude Code) | ~75 min | Skills, hooks, real projects |
| **Nick Saraev** — 4-Hour Masterclass | 4 hrs | Deep technical mastery |
| **Andrew Ng × Anthropic** — Official Course | Short | Subagents, GitHub issues |

> 📖 Curated rankings: [Best Claude Code YouTube Videos 2026](https://medium.com/@rentierdigital/i-watched-25-claude-code-youtube-videos-so-you-dont-have-to-the-definitive-ranking-550aa6863840)

### Documentation & Guides
| Resource | URL |
|----------|-----|
| Official Claude Code Docs | https://docs.anthropic.com/claude-code |
| Claude Code Skills Docs | https://code.claude.com/docs/en/skills |
| Complete Guide to Building Skills (PDF) | https://resources.anthropic.com/hubfs/The-Complete-Guide-to-Building-Skill-for-Claude.pdf |
| ClaudeLog Tutorials | https://claudelog.com/claude-code-tutorial/ |
| Claude Code Best Practices 2026 | https://www.morphllm.com/claude-code-best-practices |

### SpecKit Resources
| Resource | URL |
|----------|-----|
| GitHub: spec-kit toolkit | https://github.com/github/spec-kit |
| SpecKit + Claude Code Skills discussion | https://github.com/github/spec-kit/discussions/991 |
| Claude Code + SpecKit Method (article) | https://levelup.gitconnected.com/how-to-build-software-that-actually-works-the-claude-code-speckit-method-e62ce90d26af |
| Spec-Driven Dev with Claude Code (Medium) | https://heeki.medium.com/using-spec-driven-development-with-claude-code-4a1ebe5d9f29 |
| SpecKit Guide (ClaudeWorld) | https://claude-world.com/articles/speckit-guide/ |
| claude-code-spec-workflow (GitHub) | https://github.com/Pimzino/claude-code-spec-workflow |

---

## 📅 Week 1 — Foundations

---

### Day 1 — Monday · 30 min
**Theme: Install & First Contact**

#### Goals
- Install Claude Code and run your very first command
- Understand what Claude Code is and what it can and cannot do

#### Activities
1. **Install Claude Code** (10 min)
   - Open terminal and run: `npm install -g @anthropic-ai/claude-code`
   - Run `claude` to launch — log in with your Anthropic account
   - Try: `claude "explain what you can help me with"`

2. **Read: What is Claude Code?** (10 min)
   - Read the official overview at https://docs.anthropic.com/claude-code
   - Focus on: what it is, how it reads your codebase, what "agentic" means

3. **Explore safely** (10 min)
   - In a new empty folder, ask Claude to: *"Create a simple HTML page that says Hello World"*
   - Watch what it generates — read the file it creates

#### ✅ Done when you can
- [ ] Launch Claude Code from your terminal
- [ ] See it generate a file on request
- [ ] Understand the difference between Claude chat and Claude Code

---

### Day 2 — Tuesday · 30 min
**Theme: CLAUDE.md — Your Project Memory File**

#### Goals
- Understand why CLAUDE.md exists and how Claude Code uses it
- Write your first CLAUDE.md file

#### Activities
1. **Read the ClaudeLog guide on CLAUDE.md** (10 min)
   - https://claudelog.com/claude-code-tutorial/
   - Key ideas: CLAUDE.md is read at the start of every session; it gives Claude persistent context

2. **Read: Claude Code Best Practices (2026 Guide)** (5 min)
   - https://www.morphllm.com/claude-code-best-practices
   - Focus only on the CLAUDE.md sections

3. **Write your first CLAUDE.md** (15 min)
   - Create a new project folder: `mkdir my-first-app && cd my-first-app`
   - Create `CLAUDE.md` and write the following sections:

```markdown
# Project: My First App

## Purpose
A simple web app to track items (CRUD).

## Tech Stack
- HTML, CSS, JavaScript (no frameworks for now)
- In-memory data (no database yet)

## Coding Conventions
- Use const/let, no var
- Comment every function
- Keep files under 200 lines

## Important Notes
- Always ask before deleting anything
- Show me a plan before writing code
```

#### Key Concepts to Understand
- **Root CLAUDE.md** — applies to your whole project
- **Sub-directory CLAUDE.md** — applies to just that folder (useful later)
- CLAUDE.md is NOT just documentation — Claude Code actively reads and follows it

#### ✅ Done when you can
- [ ] Explain in your own words why CLAUDE.md matters
- [ ] Have a working CLAUDE.md file in a project folder
- [ ] Confirm Claude Code references it in a session (ask: *"What project are we working on?"*)

---

### Day 3 — Wednesday · 30 min
**Theme: Anthropic Academy — Claude Code in Action (Part 1)**

#### Goals
- Begin the official Claude Code in Action course from Anthropic Academy
- Understand Claude Code's core workflow: plan → edit → test

#### Activities
1. **Sign up for Anthropic Academy** (5 min)
   - Go to https://anthropic.skilljar.com/
   - Create a free account (email only)
   - Find "Claude Code in Action" and enroll

2. **Complete the first half of the course** (25 min)
   - Watch/read through the first modules
   - Focus on: the planning phase, how Claude reads files, how it edits code
   - Take brief notes on any commands or patterns you see

#### Key Concepts to Watch For
- How Claude Code navigates a codebase
- The difference between **chat mode** and **plan mode**
- How Claude proposes changes before making them

#### ✅ Done when you can
- [ ] Describe the basic Claude Code session loop in your own words
- [ ] Name at least 3 things Claude Code can do autonomously
- [ ] Progress at least 50% through the Anthropic Academy course

---

### Day 4 — Thursday · 30 min
**Theme: Anthropic Academy — Claude Code in Action (Part 2)**

#### Goals
- Complete the Anthropic Academy Claude Code in Action course
- Earn your certificate

#### Activities
1. **Finish the course** (20 min)
   - Complete all remaining modules
   - Pay attention to: multi-step tasks, how Claude handles errors, real-world workflows

2. **Claim your certificate** (5 min)
   - Download and save your completion certificate
   - Share it to LinkedIn if you like!

3. **Quick reflection** (5 min)
   - Write 3 things you learned in a note or journal
   - Write 1 question you still have

#### ✅ Done when you can
- [ ] Course completed and certificate downloaded
- [ ] Can describe what happens when Claude Code makes a mistake
- [ ] Have your CLAUDE.md from Day 2 open and ready to update with new knowledge

---

### Day 5 — Friday · 30 min
**Theme: Plan Mode + First Real Build**

#### Goals
- Learn to use Plan Mode to think before coding
- Follow Peter Yang's Movie App tutorial

#### Activities
1. **Watch Peter Yang's tutorial** (20 min)
   - Search YouTube: *"Claude Code Beginner's Tutorial: Build a Movie App in 15 Minutes"*
   - Also available at: https://creatoreconomy.so/p/claude-code-beginners-tutorial-build-a-movie-app-in-15-minutes
   - Pay close attention to:
     - How he uses Plan Mode before writing code
     - How he initializes `CLAUDE.md` for project memory
     - The watchlist feature implementation

2. **Try it yourself** (10 min)
   - In a new folder, ask Claude: *"Enter plan mode. I want to build a movie watchlist app with HTML and JavaScript. Before writing any code, show me your plan."*
   - Read the plan, approve it, then let Claude build

#### What Is Plan Mode?
Plan Mode tells Claude to think and outline **before** taking action. Always use it at the start of a new feature or project. You trigger it by saying *"enter plan mode"* or *"show me a plan first."*

#### ✅ Done when you can
- [ ] Use Plan Mode in a session successfully
- [ ] Have Claude generate a plan and then execute it on your approval
- [ ] Have a basic working HTML app in a folder

---

### Day 6 — Saturday · 60 min
**Theme: Nick Saraev Masterclass — Core Workflow Sections**

#### Goals
- Understand advanced Claude Code workflow patterns
- Learn about Git integration and structured project workflow

#### Activities
1. **Watch Nick Saraev's Masterclass on YouTube** (50 min)
   - Search: *"Nick Saraev Claude Code 4 Hour Masterclass"*
   - Focus on these sections (skip others for now):
     - Introduction and setup (first 15 min)
     - Workflow patterns and how he structures projects (middle sections)
     - CLAUDE.md advanced patterns
     - Skip: Git worktrees and cloud deployment (save for Week 3+)

2. **Update your CLAUDE.md** (10 min)
   - Add new rules or conventions you learned from Nick's workflow
   - Example additions:
     - Preferred file structure
     - Test requirements
     - Naming conventions

#### Key Takeaways to Watch For
- How Nick structures large tasks into smaller steps
- How he verifies Claude's output before accepting it
- How he recovers from mistakes (undo, rollback strategies)

#### ✅ Done when you can
- [ ] Describe at least 2 workflow patterns Nick uses
- [ ] Have an updated, richer CLAUDE.md file
- [ ] Know how to ask Claude to undo or rethink a change

---

### Day 7 — Sunday · 60 min
**Theme: Build Your First CRUD App (Hands-On Project)**

#### Goals
- Apply everything from Week 1 to build a real, working app
- Practice the full Claude Code workflow: CLAUDE.md → Plan Mode → Build → Verify

#### Project: Simple Item Tracker
Build a self-contained HTML + JavaScript app that lets you:
- Add items to a list (Create)
- View all items (Read)
- Edit item names (Update)
- Delete items (Delete)
- Store everything in memory (no database needed)

#### Your Workflow
1. **Create your project folder** (5 min)
   ```
   mkdir item-tracker && cd item-tracker
   ```

2. **Write your CLAUDE.md** (10 min)
   ```markdown
   # Project: Item Tracker
   ## Purpose
   A single-page CRUD app for tracking items, no backend required.
   ## Stack
   - Single HTML file with embedded CSS and JavaScript
   - In-memory array as the data store
   ## Rules
   - Keep everything in one index.html file
   - Use clear variable names
   - Add a comment above every function
   - Ask before modifying working code
   ```

3. **Use Plan Mode** (5 min)
   - Ask: *"Enter plan mode. Build me an item tracker with full CRUD using a single HTML file. Show me the plan first."*

4. **Approve and build** (20 min)
   - Review Claude's plan, ask questions if needed, then approve
   - Watch Claude write the app

5. **Test and refine** (15 min)
   - Open the HTML file in your browser
   - Ask Claude to fix any issues: *"The delete button isn't working — here's what I see..."*

6. **Reflect** (5 min)
   - What worked well? What confused you?
   - Write a short note for yourself

#### ✅ Done when you can
- [ ] Working CRUD app in your browser
- [ ] Used Plan Mode before building
- [ ] Successfully asked Claude to fix at least one issue

---

## 📅 Week 2 — Power Features

---

### Day 8 — Monday · 30 min
**Theme: Rules, Skills & SKILL.md — Deep Dive**

#### Goals
- Understand what Skills are and how they differ from CLAUDE.md
- Read the official Skills documentation

#### Activities
1. **Read the official Skills docs** (15 min)
   - https://code.claude.com/docs/en/skills
   - Key concepts:
     - A Skill = a folder with a `SKILL.md` file
     - YAML frontmatter tells Claude **when** to invoke the skill
     - Markdown content tells Claude **what to do**

2. **Read the Complete Guide to Building Skills (PDF)** (10 min)
   - https://resources.anthropic.com/hubfs/The-Complete-Guide-to-Building-Skill-for-Claude.pdf
   - Focus on: skill structure, frontmatter keywords, example skills

3. **Understand the difference** (5 min)

   | | CLAUDE.md | SKILL.md |
   |---|---|---|
   | Scope | Whole project always | Triggered on specific tasks |
   | Location | Project root | `.claude/skills/<name>/` |
   | Purpose | Project memory & rules | Reusable task instructions |
   | Example | "Always use const" | "When I ask for a data table, format it as..." |

#### ✅ Done when you can
- [ ] Explain the difference between CLAUDE.md and a Skill
- [ ] Know how YAML frontmatter triggers a skill
- [ ] Sketch out a skill you'd find useful for your own work

---

### Day 9 — Tuesday · 30 min
**Theme: Anthropic Academy — Claude Code Skills Course**

#### Goals
- Complete the dedicated Skills course from Anthropic Academy
- Write your first real Skill

#### Activities
1. **Complete the Claude Code Skills course** (20 min)
   - Back on https://anthropic.skilljar.com/
   - Find "Claude Code Skills" and complete it
   - Focus on: skill discovery, frontmatter keywords, sharing skills across projects

2. **Write your first Skill** (10 min)
   - Create a skill for your Item Tracker project:
   ```
   mkdir -p .claude/skills/crud-helper
   ```
   - Create `.claude/skills/crud-helper/SKILL.md`:

   ```markdown
   ---
   name: CRUD Helper
   description: Helps add, edit, or delete features in this CRUD app
   triggers:
     - "add a feature"
     - "add crud"
     - "new field"
   ---

   # CRUD Helper Skill

   When asked to add a new field or feature to the item tracker:
   1. First show me the plan — what files will change and why
   2. Add the new field to the in-memory array
   3. Update the HTML to display the field
   4. Update the form to accept input for the field
   5. Test that create, read, update, delete all still work
   6. Summarize what changed
   ```

#### ✅ Done when you can
- [ ] Academy Skills course completed
- [ ] At least one SKILL.md file created in your project
- [ ] Tested that Claude recognizes and uses your skill

---

### Day 10 — Wednesday · 30 min
**Theme: SpecKit — Spec-Driven Development**

#### Goals
- Understand what Spec-Driven Development (SDD) is
- Learn the SpecKit workflow phases

#### Activities
1. **Read the SpecKit introduction** (10 min)
   - GitHub Blog intro: https://github.blog/ai-and-ml/generative-ai/spec-driven-development-with-ai-get-started-with-a-new-open-source-toolkit/
   - ClaudeWorld guide: https://claude-world.com/articles/speckit-guide/

2. **Read the Level Up Coding article** (10 min)
   - https://levelup.gitconnected.com/how-to-build-software-that-actually-works-the-claude-code-speckit-method-e62ce90d26af
   - Understand: why building without a spec leads to drift, errors, and confusion

3. **Learn the 6 SpecKit phases** (10 min)
   - **Specify** → Write a pure product specification (`feature.md`)
   - **Clarify** → Resolve any open questions before coding
   - **Plan** → Technical architecture decisions (`design.md`)
   - **Tasks** → Break plan into executable steps (`tasks.md`)
   - **Implement** → Code with full traceability
   - **Validate** → Verify code matches spec exactly

#### SpecKit's 9 Core Principles (memorise these)
1. Library-First — reusable logic lives in libraries
2. CLI Interface — features accessible via CLI
3. Test-First — tests before implementation
4. Research-Driven — back decisions with research
5. Specification Consistency — code must match spec
6. Simplicity — choose the simplest solution
7. Anti-Abstraction — don't abstract prematurely
8. Minimal Scope — build only what's specified
9. Traceability — every code change links to a task

#### ✅ Done when you can
- [ ] Explain what Spec-Driven Development is and why it matters
- [ ] List the 6 SpecKit phases from memory
- [ ] Understand why "Clarify" comes before "Plan"

---

### Day 11 — Thursday · 30 min
**Theme: SpecKit + Claude Workflows — Fly-by-Wire**

#### Goals
- Combine SpecKit's structure with Claude Code's built-in workflow system
- Set up a combined workflow for your next project

#### Activities
1. **Study the Spec-Kit Autopilot Skill** (10 min)
   - Read the GitHub discussion: https://github.com/github/spec-kit/discussions/991
   - This is a Claude Skill that watches conversations and automatically orchestrates spec-kit commands

2. **Read the claude-code-spec-workflow project** (10 min)
   - https://github.com/Pimzino/claude-code-spec-workflow
   - This provides automated spec-driven + bug-fix workflows as Claude Code commands

3. **Design your combined workflow** (10 min)

   Write this workflow guide in a `WORKFLOW.md` file in your projects:

   ```markdown
   # My Combined Workflow

   ## Starting a New Feature
   1. Tell Claude: "Enter plan mode. New feature: [describe it]"
   2. Claude generates feature.md (the spec)
   3. Review and clarify open questions
   4. Claude generates design.md (technical plan)
   5. Claude generates tasks.md (step-by-step work)
   6. Approve tasks, then: "Start implementation"
   7. Claude implements task by task, checking in after each

   ## Built-in Claude Workflows I Use
   - /plan — enter plan mode
   - /review — review recent changes
   - /undo — revert last change

   ## Guiding Rules (in CLAUDE.md)
   - Always create feature.md before writing any code
   - Never skip the Clarify phase
   - Link every code change to a task number
   ```

#### ✅ Done when you can
- [ ] Understand "fly-by-wire" — Claude auto-orchestrates spec phases
- [ ] Have a personal WORKFLOW.md document
- [ ] Know how to start a new feature using the combined approach

---

### Day 12 — Saturday · 60 min
**Theme: Sabrina Ramonov — Skills, Hooks & Real Projects**

#### Goals
- Watch Sabrina Ramonov's full Claude Code course
- Learn how to build and chain Skills with quality hooks

#### Activities
1. **Watch Sabrina Ramonov's course** (50 min)
   - Search YouTube: *"Sabrina Ramonov Claude Code full course"*
   - Also at: https://www.sabrina.dev/p/claude-code-full-course-for-beginners
   - Focus on:
     - How she creates Skills from scratch
     - What quality gate hooks are
     - How she chains multiple Skills together
     - Her approach to brand voice and consistent output

2. **Apply to your project** (10 min)
   - Add one new skill to your item tracker based on what you learned
   - Examples: a "data validation" skill, a "UI styling" skill, or a "summary report" skill

#### What Are Quality Gate Hooks?
Hooks are instructions Claude follows **before** or **after** a task — like a checklist. For example:
- Before generating any HTML: *"Always check that the form has proper labels"*
- After editing a function: *"Always verify the function is still called correctly"*

You can add these to your SKILL.md files or to CLAUDE.md.

#### ✅ Done when you can
- [ ] Sabrina's course fully watched
- [ ] One new skill added to your project
- [ ] Added at least one quality gate to a SKILL.md

---

### Day 13 — Sunday · 60 min
**Theme: Capstone Project — Data Analysis Web App**

#### Goals
- Build a complete self-contained web app that loads and analyzes a static dataset
- Use the full workflow: CLAUDE.md + Skills + SpecKit phases + Plan Mode

#### Project: Kaggle Dataset Explorer
Build a single-page HTML + JavaScript app that:
- Loads a small CSV dataset (hardcoded or embedded)
- Displays the data in a table
- Shows basic statistics (count, average, min, max)
- Has a simple filter or sort feature
- Has a clean, readable design

#### Your Full Workflow
1. **Write `feature.md`** (10 min)
   Ask Claude: *"Enter plan mode. Help me write a feature.md spec for a data analysis web app..."*

2. **Clarify phase** (5 min)
   Review Claude's clarification questions and answer them

3. **Write `design.md`** (5 min)
   Ask Claude: *"Now create a design.md with the technical architecture for this feature"*

4. **Write `tasks.md`** (5 min)
   Ask Claude: *"Break this into a tasks.md with numbered implementation steps"*

5. **Implement** (25 min)
   Ask Claude: *"Start implementing task 1"* — proceed through all tasks

6. **Validate** (10 min)
   Open in browser, test all features, ask Claude to fix any issues

#### Sample Dataset to Use
Use one of these small, easy Kaggle datasets (download the CSV):
- Iris Dataset — flower measurements
- Titanic (small version) — passenger data
- World Happiness Report — country scores

#### ✅ Done when you can
- [ ] Working data app in the browser
- [ ] feature.md, design.md, and tasks.md files exist
- [ ] All SpecKit phases completed in order
- [ ] Used at least one Skill during the build

---

### Day 14 — Monday (Week 3, Day 1) · 30 min
**Theme: Review, Reflect & Lock In Your Environment**

#### Goals
- Consolidate everything you've learned
- Set up a reusable template for all future Claude Code projects

#### Activities
1. **Review your journey** (10 min)
   - Re-read your CLAUDE.md files from both projects
   - Look at your SKILL.md files — are they good? Could they be clearer?
   - Re-read your WORKFLOW.md

2. **Create your master project template** (15 min)
   Build a reusable starter folder you can copy for any new project:

   ```
   my-project-template/
   ├── CLAUDE.md          ← Your standard rules and conventions
   ├── WORKFLOW.md        ← Your SpecKit + Claude workflow guide
   ├── .claude/
   │   └── skills/
   │       └── feature-builder/
   │           └── SKILL.md   ← Your feature-building skill
   └── specs/
       ├── feature.md     ← Template spec file
       ├── design.md      ← Template design file
       └── tasks.md       ← Template tasks file
   ```

3. **Set your next learning goals** (5 min)
   Suggested Week 3+ topics:
   - [ ] MCP Development (Anthropic Academy)
   - [ ] Andrew Ng × Anthropic course — Subagents & GitHub integration
   - [ ] Advanced MCP: connecting Claude to external APIs
   - [ ] Git worktrees for parallel Claude sessions (Nick Saraev advanced section)
   - [ ] Deploy a web app built with Claude Code to a real server

#### ✅ Done when you can
- [ ] Master template folder created
- [ ] Can start a new Claude Code project in under 5 minutes
- [ ] Have a written list of your Week 3 learning goals

---

## 🧠 Key Concepts Reference Card

### CLAUDE.md
- Lives at your project root
- Read automatically at every session start
- Contains: project purpose, tech stack, coding rules, gotchas
- Use `IMPORTANT:` or `YOU MUST:` for critical rules (sparingly)
- Can have sub-directory versions for local scope

### Skills (SKILL.md)
- Live in `.claude/skills/<skill-name>/SKILL.md`
- YAML frontmatter: defines triggers (what activates the skill)
- Markdown body: instructions Claude follows when triggered
- Can be shared across projects and teams
- Think of them as reusable "playbooks" for repeated tasks

### Plan Mode
- Trigger: *"Enter plan mode"* or *"Show me a plan first"*
- Claude thinks and outlines before touching any code
- Always use at the start of a new feature or project
- Review and approve the plan before execution

### SpecKit Workflow
```
feature.md → Clarify → design.md → tasks.md → Implement → Validate
```
- Each file is a living document Claude updates as work progresses
- Implementation is always traceable back to a task number
- Spec-Kit Autopilot Skill can automate phase transitions

### Combined Workflow (Your Power Pattern)
```
CLAUDE.md (always on) + Skills (triggered) + SpecKit (per feature) + Plan Mode (per session)
```

---

## 📊 Progress Tracker

| Day | Date | Theme | Done? | Notes |
|-----|------|-------|-------|-------|
| 1 | Mon Week 1 | Install & First Run | ☐ | |
| 2 | Tue Week 1 | CLAUDE.md Fundamentals | ☐ | |
| 3 | Wed Week 1 | Anthropic Academy Part 1 | ☐ | |
| 4 | Thu Week 1 | Anthropic Academy Part 2 | ☐ | |
| 5 | Fri Week 1 | Plan Mode + Movie App | ☐ | |
| 6 | Sat Week 1 | Nick Saraev Masterclass | ☐ | |
| 7 | Sun Week 1 | Build: Item Tracker (CRUD) | ☐ | |
| 8 | Mon Week 2 | Rules, Skills & SKILL.md | ☐ | |
| 9 | Tue Week 2 | Academy: Skills Course | ☐ | |
| 10 | Wed Week 2 | SpecKit Introduction | ☐ | |
| 11 | Thu Week 2 | SpecKit + Claude Combined | ☐ | |
| 12 | Sat Week 2 | Sabrina Ramonov Course | ☐ | |
| 13 | Sun Week 2 | Capstone: Data Analysis App | ☐ | |
| 14 | Mon Week 3 | Review & Lock In Template | ☐ | |

---

## 💡 Tips for Getting the Most Out of Each Session

1. **Always start with CLAUDE.md** — Open your project, confirm Claude sees your config
2. **Plan first, code second** — Never skip Plan Mode for anything bigger than a one-liner
3. **Read before approving** — Always read what Claude plans to do before saying yes
4. **Small steps win** — Break large features into small tasks; Claude handles each one better
5. **Name your sessions** — Start each session with "We are working on [project name], [task]"
6. **Use Undo freely** — Don't be afraid to say "undo that" if something looks wrong
7. **Keep notes** — Write down patterns that work well; add them to your CLAUDE.md

---

*Plan created: March 8, 2026*
*Learner: Amit Rajpurkar*
