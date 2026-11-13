# 🔨 micro-project-tutor

**Stop taking quizzes. Learn any programming language by building one tiny real thing at a time.**

A skill for Claude that turns it into a hands-on coding tutor. It never asks "what do you know about closures?" and never hands you a multiple-choice test. Instead it gives you something to build, reads your code, and teaches exactly what your code shows you're missing.

## Why this is different

| Typical AI tutor | micro-project-tutor |
|---|---|
| "Rate your experience 1-5" | Gives you a build task and reads the code you paste |
| Quizzes and Q&A blocks | Zero quizzes. Only things to build |
| Walls of theory first | A 5-line concept flash, then you build |
| Generic exercises | Each project is a real piece of *your* end goal |
| Endless lecture | One concept per project, about 1 hour per session |

## How a session works

1. **Assess by building.** You get a small task (a styled card, a counter, a script). No hints. You paste your code.
2. **Curriculum from your gaps.** The tutor reads your code, spots what you know, what you hack around, and what's missing, then designs ~1 hour of micro-projects as a table.
3. **Flash → Build → Review.** Each micro-project: a short concept flash, a clear brief, you build, you get specific feedback (what's right, the bug, the fix).
4. **Verdict.** A table of what's solid, what you learned mid-session, and what's next.

## Install

### Claude Code

```bash
git clone https://github.com/dbdg64/micro-project-tutor.git
mkdir -p ~/.claude/skills
cp -r micro-project-tutor/skills/micro-project-tutor ~/.claude/skills/
```

Restart Claude Code. The skill triggers automatically when you say things like *"teach me Python"* or *"let's do a CSS session"*.

### Claude.ai / Claude app

Zip the `skills/micro-project-tutor` folder (so `SKILL.md` is inside the zip's top folder) and upload it under **Settings → Capabilities → Skills**. Check Anthropic's current docs if the menu has moved.

## Try it

Just say:

> teach me JavaScript

or

> Python session, I want to build a tool that renames my files

You'll get your first build task immediately. See [`examples/sample-session.md`](examples/sample-session.md) for what a session looks like.

## Works for anything

CSS, JavaScript, Python, React, Rust, Go, SQL, Bash... The skill has tuned assessment tasks for web basics, and for any other tech it picks a task that naturally exposes gaps in your fundamentals.

## Customize it

It's one Markdown file. Edit `SKILL.md` to:

- Change the session length (default ~1 hour)
- Add your own language notes under **Language Notes**
- Change the feedback format
- Set a standing end goal ("everything should be a piece of my portfolio site")

## Contributing

PRs welcome, especially:

- Assessment tasks for more languages and frameworks
- Better session-verdict formats
- Translations of the skill into other languages
- Example sessions

Open an issue if a session went badly. The transcript helps a lot.

## License

MIT. See [LICENSE](LICENSE).

---

If this helped you learn something, a ⭐ helps other learners find it.
