# Talk workspace and context

## New talk

Choose the user-requested talk root; otherwise propose a descriptively named folder separate from the plugin. Copy [starter files](../assets/starter/TALK.md) into it, preserving their relative structure. The starter's example chapter file illustrates fields; replace its unassigned entry with the real chapter outline when developed. Create working directories as their stages need them:

```text
talk/
  AGENTS.md
  TALK.md
  STATE.md
  outline/chapters.md
  outline/slides/<chapter-id>.md
  assets/originals/
  assets/ready/
  assets/index.md
  references/papers/
  references/extracts/
  references/index.md
  style/
  deck/
  output/
  tmp/
```

Fill the title, abstract, presenter, venue/date, duration, audience and intended takeaways in `TALK.md`. Unknown values remain explicitly unassigned; do not fabricate them. Resolve audience, time budget and intended contribution before committing to a detailed outline. Record the review cadence, selected profiles, supplied template, and any local style overrides. `style/` holds supplied or talk-specific guidance, not duplicated copies of all bundled references.

Use talk-root-relative paths in the brief and status. Markdown links in other files resolve relative to the containing file. Keep original downloads and usable prepared figures separate; `references/` contains evidence, `assets/` contains slide visuals, `deck/` contains editable decks, `output/` contains reviewed exports, and `tmp/` contains disposable intermediate work. Do not distribute drafts simply because they are present in `output/`; identify their status explicitly.

## Existing talk

Inspect current files first. Map its existing outlines, references, assets, style and current deck in `TALK.md`/`STATE.md`; retain its naming and locations. If several decks plausibly contain the latest manual edits, inspect content and ask which is authoritative if that cannot be established. Do not silently select by filename or timestamp.

An existing slide style guide may combine audience, writing, visuals and mechanics. Read the relevant portions and use it as local guidance without requiring a migration. A supplied reference deck establishes appearance, not facts for the new talk.

## State maintenance

Keep `STATE.md` short: stage, review status, current deck, latest reviewed output, relevant chapter paths, slide mapping, active decisions, open questions and next action. Record review scope and date; describe a draft as a draft. A superseded deck remains an archive rather than a competing current path.

Slide IDs are stable identifiers such as `S001`, independent of slide position. Map them to current positions and, when available, native PowerPoint slide IDs. After insertion/deletion/reordering, refresh that map; do not rename IDs to match numbers. Do not reuse a removed ID for different content.

At session end after substantive work, update the brief only if metadata or choices changed, update the affected outline/index entries, and refresh status. An answer-only lookup need not cause file edits. Never rely on conversation memory as the only record of a consequential decision.
