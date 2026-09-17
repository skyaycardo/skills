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

When you ask a content question mid-course, it answers from your **trusted
resources** first — website links, books, transcripts, docs you've told it to
rely on — with citations, and labels anything it adds beyond them as its own.

#### Install

```sh
git clone https://github.com/skyaycardo/skills.git
ln -s "$(pwd)/skills/tutor" ~/.agents/skills/tutor
```

(Or clone this repo directly as `~/.agents/skills` if you want it to be your
live skills directory, like I do.)

#### Getting started

On first use, the skill interviews you — what you're learning, your sources,
where you're headed, what you can practice on, and which trusted resources
(links, books, transcripts) answers should be grounded in — and writes
`context.md` itself. `context.example.md` shows the expected shape with a
filled-in example.

Trusted resources live in `trusted-resources.md` (`trusted-resources.example.md`
shows the shape), in three sections: **Knowledge** — high-trust sources,
annotated and pruned ruthlessly; **Wisdom** — communities for judgment calls;
**Gaps** — topics the destination needs that no resource covers yet. When you
ask a question, the tutor consults Knowledge first and cites it; anything it
adds beyond that is clearly labeled and anchored to a canonical source where
one exists — and it never invents a citation. Full transcripts you hand over
are stored under `trusted-resources/`.

`context.md`, `progress.md`, `trusted-resources.md`, and `trusted-resources/`
are gitignored — they're personal, and the skill recreates them if missing.

## Credits

Parts of the tutor's trusted-resources design — the high-trust curation rules,
the Knowledge / Wisdom / Gaps split, and length-matched quiz options — were
inspired by [Matt Pocock's `teach`
skill](https://github.com/mattpocock/skills/tree/main/skills/productivity/teach)
in [mattpocock/skills](https://github.com/mattpocock/skills).
