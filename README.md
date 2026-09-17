# skills

Personal [ZCode](https://zcode.com) skills. Each directory under this repo is a
self-contained skill: a `SKILL.md` (the process) plus optional reference files.

## Skills

### [`tutor/`](tutor/) — active-recall tutor for whatever you're studying

Point it at any learning material (video courses, textbooks, lectures). Share a
transcript or say you finished a lesson, and it responds with an exercise set:
closed-book **recall**, a **predict** scenario the source didn't cover, a
**diagnose** scenario ("this broke — most likely causes, most probable first"),
hands-on **practice** on your machine, and a one-line **connect** that maps the
concept to your actual goal. Answers come after the divider; send yours back and
it grades them and queues misses for spaced repetition later.

#### Install

```sh
git clone https://github.com/skyaycardo/skills.git
ln -s "$(pwd)/skills/tutor" ~/.agents/skills/tutor
```

(Or clone this repo directly as `~/.agents/skills` if you want it to be your
live skills directory, like I do.)

#### Getting started

On first use, the skill interviews you — what you're learning, your sources,
where you're headed, what you can practice on — and writes `context.md` itself.
`context.example.md` shows the expected shape with a filled-in example.

`context.md` (your profile) and `progress.md` (your history) are gitignored —
they're personal, and the skill recreates them if missing.
