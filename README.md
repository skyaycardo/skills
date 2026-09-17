# skills

My personal skills. Each folder is one skill: a
`SKILL.md` with the process and a few support files.

## [tutor/](tutor/) — an active-recall tutor for whatever you're studying

Share a transcript or say you finished a lesson, and it gives you an exercise
set: recall questions, a scenario to predict, a failure to diagnose, hands-on
practice on your machine, and a one-line tie back to why you're learning this
at all. Send your answers back and it grades them — misses go into a re-test
queue so old material comes around again.

Ask it a question mid-course and it answers from your trusted resources first
(links, books, transcripts you've told it to rely on), with citations. Anything
it adds from its own knowledge comes after, clearly labeled as such.

### Install

```sh
git clone https://github.com/skyaycardo/skills.git
ln -s "$(pwd)/skills/tutor" ~/.agents/skills/tutor
```

Or clone the repo straight into `~/.agents/skills` so it's your live skills
directory, like I do.

### Getting started

On first use it interviews you: what you're learning, your sources, your goal,
what you can practice on, and any trusted resources you want answers grounded
in. It writes `context.md` and `trusted-resources.md` itself from your answers.
The `*.example.md` files show what those look like filled in.

`context.md`, `progress.md`, `trusted-resources.md` and the transcripts under
`trusted-resources/` are all gitignored — they're personal, and the skill
recreates them if missing.

## Credits

The tutor takes some inspiration from
[Matt Pocock's skills](https://github.com/mattpocock/skills).
